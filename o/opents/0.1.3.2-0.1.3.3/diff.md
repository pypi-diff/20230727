# Comparing `tmp/opents-0.1.3.2-py3-none-any.whl.zip` & `tmp/opents-0.1.3.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,18 @@
-Zip file size: 9232 bytes, number of entries: 14
+Zip file size: 10394 bytes, number of entries: 16
 -rw-rw-r--  2.0 unx       54 b- defN 23-Jun-20 07:42 opents/__init__.py
 -rw-rw-r--  2.0 unx       14 b- defN 23-Jun-20 07:42 opents/data/__init__.py
 -rw-rw-r--  2.0 unx       31 b- defN 23-Jul-25 07:22 opents/datasets/__init__.py
--rw-rw-r--  2.0 unx     6800 b- defN 23-Jul-25 11:51 opents/datasets/datasets.py
+-rw-rw-r--  2.0 unx     6805 b- defN 23-Jul-26 03:06 opents/datasets/datasets.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jul-17 07:06 opents/evaluate/__init__.py
--rw-rw-r--  2.0 unx       23 b- defN 23-Jul-24 12:48 opents/nn/__init__.py
--rw-rw-r--  2.0 unx       20 b- defN 23-Jul-24 12:14 opents/nn/models/__init__.py
--rw-rw-r--  2.0 unx     3861 b- defN 23-Jul-25 07:05 opents/nn/models/fcn.py
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-25 12:11 opents/utils/__init__.py
--rw-rw-r--  2.0 unx    10171 b- defN 23-Jul-25 12:53 opents/utils/data_utils.py
--rw-rw-r--  2.0 unx     2198 b- defN 23-Jul-25 13:28 opents-0.1.3.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-25 13:28 opents-0.1.3.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Jul-25 13:28 opents-0.1.3.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1101 b- defN 23-Jul-25 13:28 opents-0.1.3.2.dist-info/RECORD
-14 files, 24464 bytes uncompressed, 7394 bytes compressed:  69.8%
+-rw-rw-r--  2.0 unx      113 b- defN 23-Jul-26 09:45 opents/nn/__init__.py
+-rw-rw-r--  2.0 unx       78 b- defN 23-Jul-26 09:45 opents/nn/components/__init__.py
+-rw-rw-r--  2.0 unx      777 b- defN 23-Jul-26 09:37 opents/nn/components/components.py
+-rw-rw-r--  2.0 unx       21 b- defN 23-Jul-26 09:41 opents/nn/models/__init__.py
+-rw-rw-r--  2.0 unx     3342 b- defN 23-Jul-26 11:36 opents/nn/models/fcn.py
+-rw-rw-r--  2.0 unx      116 b- defN 23-Jul-27 07:19 opents/utils/__init__.py
+-rw-rw-r--  2.0 unx    11898 b- defN 23-Jul-27 07:18 opents/utils/data_utils.py
+-rw-rw-r--  2.0 unx     2198 b- defN 23-Jul-27 08:59 opents-0.1.3.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-27 08:59 opents-0.1.3.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Jul-27 08:59 opents-0.1.3.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1280 b- defN 23-Jul-27 08:59 opents-0.1.3.3.dist-info/RECORD
+16 files, 26826 bytes uncompressed, 8272 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -12,32 +12,38 @@
 
 Filename: opents/evaluate/__init__.py
 Comment: 
 
 Filename: opents/nn/__init__.py
 Comment: 
 
+Filename: opents/nn/components/__init__.py
+Comment: 
+
+Filename: opents/nn/components/components.py
+Comment: 
+
 Filename: opents/nn/models/__init__.py
 Comment: 
 
 Filename: opents/nn/models/fcn.py
 Comment: 
 
 Filename: opents/utils/__init__.py
 Comment: 
 
 Filename: opents/utils/data_utils.py
 Comment: 
 
-Filename: opents-0.1.3.2.dist-info/METADATA
+Filename: opents-0.1.3.3.dist-info/METADATA
 Comment: 
 
-Filename: opents-0.1.3.2.dist-info/WHEEL
+Filename: opents-0.1.3.3.dist-info/WHEEL
 Comment: 
 
-Filename: opents-0.1.3.2.dist-info/top_level.txt
+Filename: opents-0.1.3.3.dist-info/top_level.txt
 Comment: 
 
-Filename: opents-0.1.3.2.dist-info/RECORD
+Filename: opents-0.1.3.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## opents/datasets/datasets.py

```diff
@@ -136,8 +136,9 @@
     def __init__(self, dataset_name, dataset_root_path=None, datasets_name=None):
         super().__init__(dataset_name, dataset_root_path, datasets_name)
         self.datasets_name = datasets_name
         self.x_train, self.y_train, self.x_test, self.y_test = self.ts_dataset()
     
     def load(self):
         return self.x_train, self.y_train, self.x_test, self.y_test
-    
+
+
```

## opents/nn/__init__.py

```diff
@@ -1 +1,2 @@
-from .models import FCN
+from .models import FCN
+from .components.components import Lambda, Residual, InitializedConv1d, InitializedLinear
```

## opents/nn/models/__init__.py

 * *Ordering differences only*

```diff
@@ -1 +1 @@
-from .fcn import FCN
+from .fcn import FCN
```

## opents/nn/models/fcn.py

```diff
@@ -1,9 +1,10 @@
 import torch
 import torch.nn as nn
+from opents.nn.components.components import Lambda, Residual, InitializedLinear, InitializedConv1d
 
 class FCN(nn.Module):
     """
     Fully Connected Network (FCN) for timeseries classification.
     """
     def __init__(self, in_channels, unit_list, out_channels, num_classes, num_cnns, kernel_size=30, stride=1, dropout=0.5, padding='same'):
         """
@@ -24,82 +25,52 @@
         self.in_channels = in_channels
         self.unit_list = unit_list
         self.out_channels = out_channels
         self.num_classes = num_classes
         self.num_cnns = num_cnns
         self.kernel = kernel_size
         self.stride = stride
-        self.dropout = dropout
-        self.padding = padding
+        self.dropout = nn.Dropout(dropout)
 
+        padding_val="same" if stride == 1 else self.kernel // 2
         self.convs = nn.ModuleList()
 
+        self.convs.append(Lambda(lambda x: torch.permute(x, [0, 2, 1])))
+
         # first cnns layer
-        self.convs.append(nn.Conv1d(self.in_channels, self.unit_list[0], kernel_size=self.kernel, stride=self.stride, padding=self.padding if self.stride == 1 else self.kernel // 2))
+        self.convs.append(InitializedConv1d(self.in_channels, self.unit_list[0], kernel_size=self.kernel, stride=self.stride, padding=padding_val))
         self.convs.append(nn.ReLU())
-        self.convs.append(nn.Dropout(self.dropout))
+        self.convs.append(self.dropout)
 
         # other cnns layers: except first cnns layer
         for unit_num in range(len(self.unit_list)):
             for cnns_num in range(self.num_cnns):
-                    self.convs.append(Residual(nn.Conv1d(self.unit_list[unit_num], self.unit_list[unit_num], kernel_size=self.kernel, padding=self.padding)))
+                    self.convs.append(Residual(InitializedConv1d(self.unit_list[unit_num], self.unit_list[unit_num], kernel_size=self.kernel, padding=padding_val)))
                     self.convs.append(nn.ReLU())
-                    self.convs.append(nn.Dropout(self.dropout))
+                    self.convs.append(self.dropout)
             if unit_num == len(self.unit_list) - 1:
                  break
-            self.convs.append(nn.Conv1d(self.unit_list[unit_num], self.unit_list[unit_num + 1], kernel_size=self.kernel, stride=self.stride, padding=self.padding))
+            self.convs.append(InitializedConv1d(self.unit_list[unit_num], self.unit_list[unit_num + 1], kernel_size=self.kernel, stride=self.stride, padding=padding_val))
             self.convs.append(nn.ReLU())
-            self.convs.append(nn.Dropout(self.dropout))
-        
-        # the last linear layer
-        self.fc = nn.Linear(unit_list[-1] * 2, num_classes)
+            self.convs.append(self.dropout)
+
+        self.convs.append(Lambda(lambda x: torch.permute(x, [0, 2, 1])))
+        self.convs.append(Lambda(lambda x: torch.concat([x.mean(dim=1), x.max(dim=1)[0]], dim=-1)))
+        self.convs.append(self.dropout) 
+
+        # add the last linear layer
+        self.convs.append(InitializedLinear(unit_list[-1] * 2, num_classes))
     
     def forward(self, inputs):
         """
         Defines the computation performed at every call.
 
         Args:
             inputs (torch.Tensor): Input tensor.
 
         Returns:
             torch.Tensor: Output tensor after passing through the network.
         """
         x = inputs
-        x = x.transpose(1, 2)
-        
         for layer in self.convs:
             x = layer(x)
-        x = x.transpose(1, 2)
-
-        # last layer
-        x = torch.cat([x.mean(dim=1), x.max(dim=1)[0]], dim=-1)
-        x = nn.Dropout(0.5)(x)
-        x = self.fc(x)
-
         return x
-
-class Residual(nn.Module):
-    """
-    Implements the Residual Block for the FCN.
-    """
-    def __init__(self, model):
-        """
-        Constructor for the Residual class.
-
-        Args:
-            model (nn.Module): The base model/block on which residual connections will be used.
-        """
-        super().__init__()
-        self.model = model
-
-    def forward(self, x):
-        """
-        Defines the computation performed at every call.
-
-        Args:
-            x (torch.Tensor): Input tensor.
-
-        Returns:
-            torch.Tensor: Output tensor after adding the input tensor and the output from the base model/block.
-        """
-        h = self.model(x)
-        return x + h
```

## opents/utils/__init__.py

```diff
@@ -1 +1 @@
-from .data_utils import RandomSplitOpenDataset, RandomSplitOpenAllDataset, relabel_from_zero
+from .data_utils import RandomSplitOpenDataset, RandomSplitOpenAllDataset, relabel_from_zero, preprocess_test_labels
```

## opents/utils/data_utils.py

```diff
@@ -128,27 +128,31 @@
     """
     def __init__(
             self,
             x_train,
             y_train,
             x_test,
             y_test,
-            train_size_rate=0.5,
+            train_size_rate=0.3,
+            test_size_rate=0.3,
             open_label_rate=0.5,
             train_random_state=42,
+            test_random_state=42,
             open_random_state=42
             ):
         
         self.x_train = x_train
         self.y_train = y_train
         self.x_test = x_test
         self.y_test = y_test
         self.train_size_rate = train_size_rate
+        self.test_size_rate = test_size_rate
         self.open_label_rate = open_label_rate
         self.train_random_state = train_random_state
+        self.test_random_state = test_random_state
         self.open_random_state = open_random_state
         
         self.x_train, self.y_train, self.x_test, self.y_test = x_train.numpy(), y_train.numpy(), x_test.numpy(), y_test.numpy()
 
     def load(self):
         """
         Loads the dataset and splits it into training and testing sets.
@@ -162,30 +166,31 @@
         unique_labels = np.unique(self.all_labels)
         y_open_nums = int(len(unique_labels) * self.train_size_rate)
 
         # if the number of y_open is 0, it indicates that the dataset has not open data.
         if y_open_nums == 0:
             raise ValueError("The number of open label data is 0, please change the percentage.")
 
-        # fix the seed of random
         random.seed(self.train_random_state)
-
         # choose the y_open and unselected_labels in y_all. the labels in the y_open and unselected_labels are unique. 
         self.selected_open_labels = random.sample(list(unique_labels), y_open_nums)
         unselected_labels = [_ for _ in unique_labels if _ not in self.selected_open_labels]
 
-        x_train, x_test, y_train, y_test = train_test_split(self.all_features, self.all_labels, train_size=self.train_size_rate, random_state=self.train_random_state, stratify=self.all_labels)
+        self.x_train_val, x_test, self.y_train_val, y_test = train_test_split(self.all_features, self.all_labels, train_size= 1 - self.test_size_rate, random_state=self.train_random_state, stratify=self.all_labels)
+        
+        x_train, x_val, y_train, y_val = train_test_split(self.x_train_val, self.y_train_val, train_size=self.train_size_rate / (1 - self.test_size_rate), random_state=self.test_random_state, stratify=self.y_train_val)
 
-        mask = np.isin(y_train, self.selected_open_labels, invert=True)
-        x_train = x_train[mask]
-        y_train = y_train[mask]
+        train_mask = np.isin(y_train, self.selected_open_labels, invert=True)
+        val_mask = np.isin(y_val, self.selected_open_labels, invert=True)
+        x_train, x_val = x_train[train_mask], x_val[val_mask]
+        y_train, y_val = y_train[train_mask], y_val[val_mask]
         
-        x_train, y_train, x_test, y_test = torch.tensor(x_train), torch.tensor(y_train).long(), torch.tensor(x_test), torch.tensor(y_test).long()
+        x_train, y_train, x_val, y_val, x_test, y_test = torch.tensor(x_train), torch.tensor(y_train).long(), torch.tensor(x_val), torch.tensor(y_val).long(), torch.tensor(x_test), torch.tensor(y_test).long()
 
-        return x_train, y_train, x_test, y_test
+        return x_train, y_train, x_val, y_val, x_test, y_test
         
 class RandomSplitOpenAllDataset(RandomSplitOpenDataset):
     def __init__(self, x_train, y_train, x_test, y_test, train_size_rate, open_label_rate, train_random_state=42, open_random_state=42):
         super().__init__(x_train, y_train, x_test, y_test, train_size_rate, open_label_rate, train_random_state, open_random_state)
     
     def load(self):
         x_train, y_train, x_test, y_test = super().load()
@@ -215,8 +220,43 @@
         return labels
     if len(args) == 2:
         y_train, y_test = args[0].numpy(), args[1].numpy()
         encoder.fit(np.concatenate([y_train, y_test]))
         y_train = encoder.transform(y_train)
         y_test = encoder.transform(y_test)
         y_train, y_test = torch.tensor(y_train).long(),torch.tensor(y_test).long()
-        return y_train, y_test
+        return y_train, y_test
+
+def preprocess_test_labels(y_test, y_train, real_label):
+    """
+    Function to preprocess test labels: 
+    replace labels in `real_label` with the corresponding labels in y_train, 
+    and assign new labels to the rest
+
+    Args:
+    y_test (torch.Tensor): Test labels to be preprocessed
+    y_train (torch.Tensor): Training labels used for mapping
+    real_label (torch.Tensor): Real labels in training set
+
+    Returns:
+    torch.Tensor: Preprocessed test labels
+    """
+
+    # Convert to list for easy manipulation
+    real_label_list = real_label.tolist()
+    y_train_unique = torch.unique(y_train).tolist()
+
+    # Create a mapping from real_label to the corresponding y_train labels
+    label_mapping = {real_label_list[i]: y_train_unique[i] for i in range(len(real_label_list))}
+
+    # Maximum label in y_train
+    max_train_label = max(y_train_unique)
+
+    def relabel_test(y):
+        if y.item() in real_label_list:
+            return label_mapping[y.item()]
+        else:
+            return max_train_label + 1
+
+    y_test_preprocessed = torch.tensor([relabel_test(y) for y in y_test])
+
+    return y_test_preprocessed
```

## Comparing `opents-0.1.3.2.dist-info/METADATA` & `opents-0.1.3.3.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opents
-Version: 0.1.3.2
+Version: 0.1.3.3
 Summary: OpenTS is a friendly Python Library for time series analysis
 Home-page: https://github.com/PyOpenTS/PyOpenTS
 Author: hushuguo
 Author-email: husg8217@mails.jlu.edu.cn
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: torch
```

## Comparing `opents-0.1.3.2.dist-info/RECORD` & `opents-0.1.3.3.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 opents/__init__.py,sha256=xRL8tSUxNiTSIygSIrQ0Y2i_guxRW_SNhljbNkCKNP4,54
 opents/data/__init__.py,sha256=E_iP2Kb-in3dJvXIMmvTbcBz6OrHVHDGFEwC-Qakdj0,14
 opents/datasets/__init__.py,sha256=Il-hXgnDs4L3Afz9rCX_OY_y4JSInjBMGn0kcJbV4jY,31
-opents/datasets/datasets.py,sha256=oRYDZO-JrV6zSZuHN0vOsgxQjhq5FWUhYFem7e7vxE4,6800
+opents/datasets/datasets.py,sha256=_04nLAjj7QaSSJSexaZSdTI5Ahkwsq7lJ4MFP8Gn4kI,6805
 opents/evaluate/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-opents/nn/__init__.py,sha256=6uEDX0GQ3Z3aaZsVf3r9dnlWK2k-VeWh3uqEqHgA8vo,23
-opents/nn/models/__init__.py,sha256=b1LlF1f44wRZ4S4cGD7jT4TXHs3CEHJv-Q3ylsK8O-E,20
-opents/nn/models/fcn.py,sha256=N1s0JQyj_V4LiueWLY-ZZhTMpOIEqyJ4vXmRktplhnk,3861
-opents/utils/__init__.py,sha256=yz0eMqw6MGe9pEgENz1hCRkJgtYeVuOEtObEKHKorUs,92
-opents/utils/data_utils.py,sha256=dyQ9eK49ef16LwiyDpXrxr7_8-4eg40t48VXuAiJHr8,10171
-opents-0.1.3.2.dist-info/METADATA,sha256=8RQbB_KHQiftp96gXxtevJZcmezqcWgwg7TY2ED3D44,2198
-opents-0.1.3.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-opents-0.1.3.2.dist-info/top_level.txt,sha256=VMPO4pjOtyRL1h-EZc31aY2v5787ZqAKkOzzbkgw300,7
-opents-0.1.3.2.dist-info/RECORD,,
+opents/nn/__init__.py,sha256=j3IdJ91w6qCt4N8y_6Ly9M0vyn09zHyyfDNAKNK_6Vg,113
+opents/nn/components/__init__.py,sha256=A9lO17mKCekE8pwOoI6_L---59zRMkv6b-PL6aS0O9c,78
+opents/nn/components/components.py,sha256=IP0Mylqm42mqLo-iBVg8_aRoXVaTAB0EgABZVMHrCDc,777
+opents/nn/models/__init__.py,sha256=8-UOa7bnfrurKHPk8ffpbMaYxw93PSrQ994pl72exa0,21
+opents/nn/models/fcn.py,sha256=wDkkSYM8gmvhShc86fJNCYU5xmm8-2KxqqiJw0mkC-U,3342
+opents/utils/__init__.py,sha256=RWPZjD-FGxuMk99ub4oCSkOiO_wUKz3j8KLLhXo6mzw,116
+opents/utils/data_utils.py,sha256=UJFNq0YV8ROJVoam9QoJpL8nNQZnE3Sx4DklQ0DHCfs,11898
+opents-0.1.3.3.dist-info/METADATA,sha256=USKGyEVtGexTGphd_MCiQAzJvX2cHMuN3uW81ly03yk,2198
+opents-0.1.3.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+opents-0.1.3.3.dist-info/top_level.txt,sha256=VMPO4pjOtyRL1h-EZc31aY2v5787ZqAKkOzzbkgw300,7
+opents-0.1.3.3.dist-info/RECORD,,
```

