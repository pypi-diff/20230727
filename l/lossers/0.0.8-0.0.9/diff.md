# Comparing `tmp/lossers-0.0.8.tar.gz` & `tmp/lossers-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lossers-0.0.8.tar", last modified: Sun Jul 16 04:39:10 2023, max compression
+gzip compressed data, was "lossers-0.0.9.tar", last modified: Thu Jul 27 14:31:36 2023, max compression
```

## Comparing `lossers-0.0.8.tar` & `lossers-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:39:10.483449 lossers-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-16 04:38:59.000000 lossers-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-16 04:39:10.483449 lossers-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-16 04:38:59.000000 lossers-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:39:10.479449 lossers-0.0.8/lossers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:59.000000 lossers-0.0.8/lossers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-16 04:38:59.000000 lossers-0.0.8/lossers/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-16 04:38:59.000000 lossers-0.0.8/lossers/gan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:39:10.483449 lossers-0.0.8/lossers/lpips/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-16 04:38:59.000000 lossers-0.0.8/lossers/lpips/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-07-16 04:38:59.000000 lossers-0.0.8/lossers/lpips/lpips.py
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-07-16 04:38:59.000000 lossers-0.0.8/lossers/lpips/pretrained_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-07-16 04:38:59.000000 lossers-0.0.8/lossers/lpips/vgg_v0.1.pth
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-16 04:38:59.000000 lossers-0.0.8/lossers/math.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-16 04:38:59.000000 lossers-0.0.8/lossers/softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-16 04:38:59.000000 lossers-0.0.8/lossers/ssim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:39:10.483449 lossers-0.0.8/lossers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-16 04:39:10.000000 lossers-0.0.8/lossers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-16 04:39:10.000000 lossers-0.0.8/lossers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 04:39:10.000000 lossers-0.0.8/lossers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-16 04:39:10.000000 lossers-0.0.8/lossers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 04:39:10.483449 lossers-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-16 04:38:59.000000 lossers-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:31:36.338603 lossers-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-27 14:31:25.000000 lossers-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-27 14:31:36.338603 lossers-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-27 14:31:25.000000 lossers-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:31:36.338603 lossers-0.0.9/lossers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:31:25.000000 lossers-0.0.9/lossers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-27 14:31:25.000000 lossers-0.0.9/lossers/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-27 14:31:25.000000 lossers-0.0.9/lossers/gan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:31:36.338603 lossers-0.0.9/lossers/lpips/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-27 14:31:25.000000 lossers-0.0.9/lossers/lpips/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-07-27 14:31:25.000000 lossers-0.0.9/lossers/lpips/lpips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-07-27 14:31:25.000000 lossers-0.0.9/lossers/lpips/pretrained_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-07-27 14:31:25.000000 lossers-0.0.9/lossers/lpips/vgg_v0.1.pth
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-27 14:31:25.000000 lossers-0.0.9/lossers/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-27 14:31:25.000000 lossers-0.0.9/lossers/softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-27 14:31:25.000000 lossers-0.0.9/lossers/ssim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:31:36.338603 lossers-0.0.9/lossers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-27 14:31:36.000000 lossers-0.0.9/lossers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-27 14:31:36.000000 lossers-0.0.9/lossers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 14:31:36.000000 lossers-0.0.9/lossers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-27 14:31:36.000000 lossers-0.0.9/lossers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 14:31:36.338603 lossers-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-27 14:31:25.000000 lossers-0.0.9/setup.py
```

### Comparing `lossers-0.0.8/LICENSE` & `lossers-0.0.9/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Mr. Zhang
+Copyright (c) 2023 Jiau Zhang
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `lossers-0.0.8/PKG-INFO` & `lossers-0.0.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lossers
-Version: 0.0.8
+Version: 0.0.9
 Summary: Deep Learning Loss Function
 Home-page: https://github.com/JiauZhang/lossers
 Author: JiauZhang
 Author-email: jiauzhang@163.com
 License: MIT
 Keywords: Deep Learning,Loss Function,Artificial Intelligence
 Classifier: Intended Audience :: Developers
```

### Comparing `lossers-0.0.8/lossers/gan.py` & `lossers-0.0.9/lossers/gan.py`

 * *Files identical despite different names*

### Comparing `lossers-0.0.8/lossers/lpips/lpips.py` & `lossers-0.0.9/lossers/lpips/lpips.py`

 * *Files identical despite different names*

### Comparing `lossers-0.0.8/lossers/lpips/pretrained_model.py` & `lossers-0.0.9/lossers/lpips/pretrained_model.py`

 * *Files identical despite different names*

### Comparing `lossers-0.0.8/lossers/lpips/vgg_v0.1.pth` & `lossers-0.0.9/lossers/lpips/vgg_v0.1.pth`

 * *Files identical despite different names*

### Comparing `lossers-0.0.8/lossers/softmax.py` & `lossers-0.0.9/lossers/softmax.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,12 +13,12 @@
         self.in_dims = in_dims
         self.weight = nn.Parameter(torch.randn(n_classes, in_dims), requires_grad=True)
         nn.init.xavier_normal_(self.weight, gain=1)
 
     def forward(self, logits, labels):
         cosine = F_.linear(F_.normalize(logits), F_.normalize(self.weight))
         labels_view = labels.view(-1, 1)
-        delta_cosine = torch.zeros(cosine.size()).scatter_(1, labels_view, self.m)
+        delta_cosine = torch.zeros_like(cosine).scatter_(1, labels_view, self.m)
         cosine_m = cosine - delta_cosine
         cosine_ms = self.s * cosine_m
         loss = F_.cross_entropy(cosine_ms, labels)
         return loss
```

### Comparing `lossers-0.0.8/lossers/ssim.py` & `lossers-0.0.9/lossers/ssim.py`

 * *Files identical despite different names*

### Comparing `lossers-0.0.8/lossers.egg-info/PKG-INFO` & `lossers-0.0.9/lossers.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lossers
-Version: 0.0.8
+Version: 0.0.9
 Summary: Deep Learning Loss Function
 Home-page: https://github.com/JiauZhang/lossers
 Author: JiauZhang
 Author-email: jiauzhang@163.com
 License: MIT
 Keywords: Deep Learning,Loss Function,Artificial Intelligence
 Classifier: Intended Audience :: Developers
```

### Comparing `lossers-0.0.8/setup.py` & `lossers-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'lossers',
     packages = find_packages(exclude=['examples']),
     package_data={'': ['*/vgg_v0.1.pth']},
-    version = '0.0.8',
+    version = '0.0.9',
     license='MIT',
     description = 'Deep Learning Loss Function',
     author = 'JiauZhang',
     author_email = 'jiauzhang@163.com',
     url = 'https://github.com/JiauZhang/lossers',
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type = 'text/markdown',
```

