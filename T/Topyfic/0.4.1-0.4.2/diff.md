# Comparing `tmp/Topyfic-0.4.1.tar.gz` & `tmp/Topyfic-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Topyfic-0.4.1.tar", last modified: Mon Jul 24 20:52:14 2023, max compression
+gzip compressed data, was "Topyfic-0.4.2.tar", last modified: Wed Jul 26 22:24:51 2023, max compression
```

## Comparing `Topyfic-0.4.1.tar` & `Topyfic-0.4.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2023-07-24 20:52:14.447967 Topyfic-0.4.1/
--rw-r--r--   0 nargesrezaie   (501) staff       (20)     1067 2022-01-27 20:57:46.000000 Topyfic-0.4.1/LICENSE.txt
--rw-r--r--   0 nargesrezaie   (501) staff       (20)      903 2023-07-24 20:52:14.448052 Topyfic-0.4.1/PKG-INFO
--rw-r--r--   0 nargesrezaie   (501) staff       (20)     3280 2023-04-27 22:47:11.000000 Topyfic-0.4.1/README.md
-drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2023-07-24 20:52:14.446776 Topyfic-0.4.1/Topyfic/
--rw-rw-r--   0 nargesrezaie   (501) staff       (20)      197 2023-06-01 18:15:16.000000 Topyfic-0.4.1/Topyfic/__init__.py
--rw-r--r--   0 nargesrezaie   (501) staff       (20)    45131 2023-07-24 20:48:04.000000 Topyfic-0.4.1/Topyfic/analysis.py
--rw-r--r--   0 nargesrezaie   (501) staff       (20)     4087 2023-06-01 18:15:16.000000 Topyfic-0.4.1/Topyfic/main.py
--rw-r--r--   0 nargesrezaie   (501) staff       (20)    13776 2023-06-05 22:53:45.000000 Topyfic-0.4.1/Topyfic/topModel.py
--rw-r--r--   0 nargesrezaie   (501) staff       (20)     8982 2023-06-01 18:15:16.000000 Topyfic-0.4.1/Topyfic/topic.py
--rw-r--r--   0 nargesrezaie   (501) staff       (20)    10440 2023-05-31 22:59:19.000000 Topyfic-0.4.1/Topyfic/train.py
--rw-r--r--   0 nargesrezaie   (501) staff       (20)    19189 2023-07-14 01:34:33.000000 Topyfic-0.4.1/Topyfic/utilsAnalyseModel.py
--rw-r--r--   0 nargesrezaie   (501) staff       (20)    21371 2023-05-31 23:11:38.000000 Topyfic-0.4.1/Topyfic/utilsMakeModel.py
-drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2023-07-24 20:52:14.447828 Topyfic-0.4.1/Topyfic.egg-info/
--rw-r--r--   0 nargesrezaie   (501) staff       (20)      903 2023-07-24 20:52:14.000000 Topyfic-0.4.1/Topyfic.egg-info/PKG-INFO
--rw-r--r--   0 nargesrezaie   (501) staff       (20)      359 2023-07-24 20:52:14.000000 Topyfic-0.4.1/Topyfic.egg-info/SOURCES.txt
--rw-r--r--   0 nargesrezaie   (501) staff       (20)        1 2023-07-24 20:52:14.000000 Topyfic-0.4.1/Topyfic.egg-info/dependency_links.txt
--rw-r--r--   0 nargesrezaie   (501) staff       (20)      280 2023-07-24 20:52:14.000000 Topyfic-0.4.1/Topyfic.egg-info/requires.txt
--rw-r--r--   0 nargesrezaie   (501) staff       (20)        8 2023-07-24 20:52:14.000000 Topyfic-0.4.1/Topyfic.egg-info/top_level.txt
--rw-r--r--   0 nargesrezaie   (501) staff       (20)       79 2023-07-24 20:52:14.448325 Topyfic-0.4.1/setup.cfg
--rw-r--r--   0 nargesrezaie   (501) staff       (20)     2018 2023-07-24 20:48:58.000000 Topyfic-0.4.1/setup.py
+drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2023-07-26 22:24:51.895823 Topyfic-0.4.2/
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)     1067 2022-01-27 20:57:46.000000 Topyfic-0.4.2/LICENSE.txt
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)      903 2023-07-26 22:24:51.895907 Topyfic-0.4.2/PKG-INFO
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)     3280 2023-04-27 22:47:11.000000 Topyfic-0.4.2/README.md
+drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2023-07-26 22:24:51.894595 Topyfic-0.4.2/Topyfic/
+-rw-rw-r--   0 nargesrezaie   (501) staff       (20)      197 2023-06-01 18:15:16.000000 Topyfic-0.4.2/Topyfic/__init__.py
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)    45313 2023-07-26 18:42:31.000000 Topyfic-0.4.2/Topyfic/analysis.py
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)     4087 2023-06-01 18:15:16.000000 Topyfic-0.4.2/Topyfic/main.py
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)    13776 2023-06-05 22:53:45.000000 Topyfic-0.4.2/Topyfic/topModel.py
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)     8982 2023-06-01 18:15:16.000000 Topyfic-0.4.2/Topyfic/topic.py
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)    10440 2023-05-31 22:59:19.000000 Topyfic-0.4.2/Topyfic/train.py
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)    19189 2023-07-14 01:34:33.000000 Topyfic-0.4.2/Topyfic/utilsAnalyseModel.py
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)    21560 2023-07-25 22:29:44.000000 Topyfic-0.4.2/Topyfic/utilsMakeModel.py
+drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2023-07-26 22:24:51.895663 Topyfic-0.4.2/Topyfic.egg-info/
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)      903 2023-07-26 22:24:51.000000 Topyfic-0.4.2/Topyfic.egg-info/PKG-INFO
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)      359 2023-07-26 22:24:51.000000 Topyfic-0.4.2/Topyfic.egg-info/SOURCES.txt
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)        1 2023-07-26 22:24:51.000000 Topyfic-0.4.2/Topyfic.egg-info/dependency_links.txt
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)      280 2023-07-26 22:24:51.000000 Topyfic-0.4.2/Topyfic.egg-info/requires.txt
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)        8 2023-07-26 22:24:51.000000 Topyfic-0.4.2/Topyfic.egg-info/top_level.txt
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)       79 2023-07-26 22:24:51.896188 Topyfic-0.4.2/setup.cfg
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)     2018 2023-07-26 22:23:04.000000 Topyfic-0.4.2/setup.py
```

### Comparing `Topyfic-0.4.1/LICENSE.txt` & `Topyfic-0.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Topyfic-0.4.1/PKG-INFO` & `Topyfic-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: Topyfic
-Version: 0.4.1
+Version: 0.4.2
 Summary: Topyfic is a Python package designed to identify reproducible latent dirichlet allocation (LDA) using leiden clustering and harmony for single cell epigenomics data
 Home-page: https://github.com/mortazavilab/Topyfic
-Download-URL: https://github.com/mortazavilab/Topyfic/archive/refs/tags/v0.4.1.tar.gz
+Download-URL: https://github.com/mortazavilab/Topyfic/archive/refs/tags/v0.4.2.tar.gz
 Author: Narges Rezaie
 Author-email: nargesrezaie80@gmail.com
 License: MIT
 Keywords: Cellular Programs,Latent Dirichlet allocation,single-cell multiome,single-cell RNA-seq,gene regulatory network,Topic Modeling,single-nucleus RNA-seq
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research 
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

### Comparing `Topyfic-0.4.1/README.md` & `Topyfic-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `Topyfic-0.4.1/Topyfic/analysis.py` & `Topyfic-0.4.2/Topyfic/analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,43 +105,49 @@
 
         if category is None:
             category = self.cell_participation.obs[level].unique().tolist()
 
         if figsize is None:
             figsize = (10 * (len(category) + 1), 10)
 
+        if self.top_model.N <= n:
+            n = max(0, self.top_model.N-2)
+
         fig, axs = plt.subplots(ncols=len(category) + 1,
                                 figsize=figsize,
                                 facecolor='white')
 
         colors = self.colors_topics
 
         if ascending is None:
             ascending = [False] * len(category)
 
         for i in range(len(category)):
+            print(i, category[i])
             tissue = self.cell_participation.obs[self.cell_participation.obs[level] == category[i]]
             tmp = self.cell_participation.to_df().loc[tissue.index, :]
-            order = tmp.mean().sort_values(ascending=False).index.tolist()
-            index = tmp[order].sort_values(by=order, ascending=False).index.tolist()
+            order = tmp.mean().sort_values(ascending=ascending[i]).index.tolist()
+            index = tmp[order].sort_values(by=order, ascending=ascending[i]).index.tolist()
             tmp = tmp.reindex(columns=order)
             tmp = tmp.reindex(index)
             colors = colors.reindex(order)
             labels = tmp.columns.tolist()
-            labels[n:] = ['' for i in range(len(labels) - 5)]
+            labels[n:] = ['' for i in range(len(labels) - n)]
 
             def make_autopct(values):
                 def my_autopct(pct):
                     if pct > values[n] * 100:
                         return '{p:.0f}%'.format(p=pct)
                     else:
                         return ''
 
                 return my_autopct
 
+            print(tmp.mean())
+            print(labels)
             axs[i].pie(tmp.mean(),
                        labels=labels,
                        colors=colors.colors.tolist(),
                        autopct=make_autopct(tmp.mean()),
                        wedgeprops={'linewidth': 0},
                        # labeldistance=0.8,
                        textprops={"fontsize": 25})
```

### Comparing `Topyfic-0.4.1/Topyfic/main.py` & `Topyfic-0.4.2/Topyfic/main.py`

 * *Files identical despite different names*

### Comparing `Topyfic-0.4.1/Topyfic/topModel.py` & `Topyfic-0.4.2/Topyfic/topModel.py`

 * *Files identical despite different names*

### Comparing `Topyfic-0.4.1/Topyfic/topic.py` & `Topyfic-0.4.2/Topyfic/topic.py`

 * *Files identical despite different names*

### Comparing `Topyfic-0.4.1/Topyfic/train.py` & `Topyfic-0.4.2/Topyfic/train.py`

 * *Files identical despite different names*

### Comparing `Topyfic-0.4.1/Topyfic/utilsAnalyseModel.py` & `Topyfic-0.4.2/Topyfic/utilsAnalyseModel.py`

 * *Files identical despite different names*

### Comparing `Topyfic-0.4.1/Topyfic/utilsMakeModel.py` & `Topyfic-0.4.2/Topyfic/utilsMakeModel.py`

 * *Files 3% similar despite different names*

```diff
@@ -304,38 +304,45 @@
     :type file_format: str
     :param file_name: name and path of the plot use for save (default: cluster_contribution)
     :type file_name: str
     """
     if feature not in clustering.columns:
         sys.exit(f"{feature} is not valid! should be a columns names of clustering")
 
-    if not show_all:
-        clustering = clustering[clustering["keep"]]
-
-    options = np.unique(clustering[feature]).tolist()
-    res = pd.DataFrame(columns=options,
+    options = np.unique(clustering['assays']).tolist()
+    res = pd.DataFrame(columns=options + ['Topic', 'keep'],
                        index=range(len(clustering['leiden'].unique())))
 
-    for i in range(res.shape[0]):
+    for i in clustering['leiden'].unique():
         for opt in options:
             tmp = clustering[np.logical_and(clustering['leiden'] == i,
-                                            clustering[feature] == opt)]
+                                            clustering['assays'] == opt)]
             res.loc[i, opt] = tmp.shape[0]
+
+        tmp = clustering[clustering['leiden'] == i]
+        res.loc[i, 'Topic'] = f"Topic_{i + 1}"
+        res.loc[i, 'keep'] = tmp.keep.unique()[0]
+
+    if not show_all:
+        res = res[res["keep"]]
+    res.index = res.Topic.values
+
     if not portion:
         plot = res.plot.bar(stacked=True,
                             xlabel='leiden',
                             ylabel='number of topics',
                             figsize=(max(res.shape[0] / 2, 5), 7))
     else:
-        sum_feature = res.sum(axis=1)
-        for i in range(res.shape[0]):
+        res['sum'] = res[options].sum(axis=1)
+        for i in res.index.values:
             for opt in options:
-                res.loc[i, opt] = res.loc[i, opt] / sum_feature[i] * 100
-        res.index = res.index + 1
-        res.index = "Topics_" + res.index.astype(str)
+                res.loc[i, opt] = float(res.loc[i, opt]) / res.loc[i, 'sum'] * 100
+
+        res.drop(['Topic', 'keep', 'sum'], axis=1, inplace=True)
+
         plot = res.plot.bar(stacked=True,
                             xlabel='leiden',
                             ylabel='percentage(%) of topics',
                             figsize=(max(res.shape[0] / 2, 5), 7))
     fig = plot.get_figure()
     if save:
         fig.savefig(f"{file_name}.{file_format}", bbox_inches='tight')
```

### Comparing `Topyfic-0.4.1/Topyfic.egg-info/PKG-INFO` & `Topyfic-0.4.2/Topyfic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: Topyfic
-Version: 0.4.1
+Version: 0.4.2
 Summary: Topyfic is a Python package designed to identify reproducible latent dirichlet allocation (LDA) using leiden clustering and harmony for single cell epigenomics data
 Home-page: https://github.com/mortazavilab/Topyfic
-Download-URL: https://github.com/mortazavilab/Topyfic/archive/refs/tags/v0.4.1.tar.gz
+Download-URL: https://github.com/mortazavilab/Topyfic/archive/refs/tags/v0.4.2.tar.gz
 Author: Narges Rezaie
 Author-email: nargesrezaie80@gmail.com
 License: MIT
 Keywords: Cellular Programs,Latent Dirichlet allocation,single-cell multiome,single-cell RNA-seq,gene regulatory network,Topic Modeling,single-nucleus RNA-seq
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research 
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

### Comparing `Topyfic-0.4.1/setup.py` & `Topyfic-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup
 
 setup(
     name='Topyfic',  # the name of your package
     packages=['Topyfic'],  # same as above
-    version='v0.4.1',  # version number
+    version='v0.4.2',  # version number
     license='MIT',  # license type
     description='Topyfic is a Python package designed to identify reproducible latent dirichlet allocation (LDA) '
                 'using leiden clustering and harmony for single cell epigenomics data',
     # short description
     author='Narges Rezaie',  # your name
     author_email='nargesrezaie80@gmail.com',  # your email
     url='https://github.com/mortazavilab/Topyfic',  # url to your git repo
-    download_url='https://github.com/mortazavilab/Topyfic/archive/refs/tags/v0.4.1.tar.gz',  # link to the tar.gz file associated with this release
+    download_url='https://github.com/mortazavilab/Topyfic/archive/refs/tags/v0.4.2.tar.gz',  # link to the tar.gz file associated with this release
     keywords=['Cellular Programs', 'Latent Dirichlet allocation', 'single-cell multiome', 'single-cell RNA-seq',
               'gene regulatory network', 'Topic Modeling', 'single-nucleus RNA-seq'],  #
     python_requires='>=3.8',
     install_requires=[  # these can also include >, <, == to enforce version compatibility
         'pandas>=1.4.4',  # make sure the packages you put here are those NOT included in the base python distribution
         'scikit-learn>=0.24.2',
         'pytest',
```

