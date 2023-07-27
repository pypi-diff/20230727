# Comparing `tmp/destinynet-0.1.0.tar.gz` & `tmp/destinynet-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "destinynet-0.1.0.tar", max compression
+gzip compressed data, was "destinynet-0.1.1.tar", max compression
```

## Comparing `destinynet-0.1.0.tar` & `destinynet-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       33 2023-07-27 05:54:27.469078 destinynet-0.1.0/DestinyNet/__init__.py
--rw-r--r--   0        0        0    12161 2023-07-27 05:52:50.073810 destinynet-0.1.0/DestinyNet/train.py
--rw-r--r--   0        0        0     2450 2023-07-27 05:33:09.658986 destinynet-0.1.0/DestinyNet/utils.py
--rw-r--r--   0        0        0      494 2023-07-27 06:06:15.190541 destinynet-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      690 1970-01-01 00:00:00.000000 destinynet-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       52 2023-07-27 06:22:58.525600 destinynet-0.1.1/DestinyNet/__init__.py
+-rw-r--r--   0        0        0    12163 2023-07-27 06:22:30.005836 destinynet-0.1.1/DestinyNet/train.py
+-rw-r--r--   0        0        0     2450 2023-07-27 05:33:09.658986 destinynet-0.1.1/DestinyNet/utils.py
+-rw-r--r--   0        0        0      494 2023-07-27 06:25:58.872117 destinynet-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      690 1970-01-01 00:00:00.000000 destinynet-0.1.1/PKG-INFO
```

### Comparing `destinynet-0.1.0/DestinyNet/train.py` & `destinynet-0.1.1/DestinyNet/train.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,15 +171,15 @@
 
     # 重写len方法获取数据集大小
     def __len__(self):
         return self.length
 
 
 
-def main(args):
+def train(args):
     device=args.device
     adata_orig = cs.hf.read(args.adata_orig)
     traincell1 = np.loadtxt(args.traincell1)
     traincell2 = np.loadtxt(args.traincell2)
     testcell1 = np.loadtxt(args.testcell1)
     testcell2 = np.loadtxt(args.testcell2)
     train_rel = np.loadtxt(args.train_rel, dtype=int)
@@ -325,8 +325,8 @@
             mapembedding.append(mapEmbedding)
     all_embeddings = np.array(all_embeddings)
     mapembedding = np.array(mapembedding)
     np.savez(args.embeddings_path, all_embeddings)
     np.savez(args.mapping_path, mapembedding)
 if __name__ == "__main__":
     args = get_args()
-    main(args)
+    train(args)
```

### Comparing `destinynet-0.1.0/DestinyNet/utils.py` & `destinynet-0.1.1/DestinyNet/utils.py`

 * *Files identical despite different names*

### Comparing `destinynet-0.1.0/PKG-INFO` & `destinynet-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: destinynet
-Version: 0.1.0
+Version: 0.1.1
 Summary: This is a code to predict cell's fate
 Author: Songtao Jiang
 Author-email: songtao.22@intl.zju.edu.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

