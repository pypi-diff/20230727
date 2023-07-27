# Comparing `tmp/labeltransform2-2.1.tar.gz` & `tmp/labeltransform2-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labeltransform2-2.1.tar", last modified: Thu Jun 15 12:12:23 2023, max compression
+gzip compressed data, was "labeltransform2-2.2.tar", last modified: Sat Jul  1 11:41:55 2023, max compression
```

## Comparing `labeltransform2-2.1.tar` & `labeltransform2-2.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 12:12:23.661352 labeltransform2-2.1/
--rw-rw-rw-   0        0        0    11558 2023-06-14 02:18:41.000000 labeltransform2-2.1/LICENSE
--rw-rw-rw-   0        0        0      225 2023-06-15 12:12:23.660354 labeltransform2-2.1/PKG-INFO
--rw-rw-rw-   0        0        0      961 2023-06-14 02:18:41.000000 labeltransform2-2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 12:12:23.653358 labeltransform2-2.1/labeltransform2/
--rw-rw-rw-   0        0        0       34 2023-06-14 07:41:09.000000 labeltransform2-2.1/labeltransform2/__init__.py
--rw-rw-rw-   0        0        0     4675 2023-06-15 06:30:34.000000 labeltransform2-2.1/labeltransform2/generate_voc.py
--rw-rw-rw-   0        0        0      896 2023-06-15 12:11:48.000000 labeltransform2-2.1/labeltransform2/tools.py
-drwxrwxrwx   0        0        0        0 2023-06-15 12:12:23.659352 labeltransform2-2.1/labeltransform2/xml/
--rw-rw-rw-   0        0        0      469 2023-06-14 03:30:14.000000 labeltransform2-2.1/labeltransform2/xml/voc.xml
-drwxrwxrwx   0        0        0        0 2023-06-15 12:12:23.658378 labeltransform2-2.1/labeltransform2.egg-info/
--rw-rw-rw-   0        0        0      225 2023-06-15 12:12:23.000000 labeltransform2-2.1/labeltransform2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      333 2023-06-15 12:12:23.000000 labeltransform2-2.1/labeltransform2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 12:12:23.000000 labeltransform2-2.1/labeltransform2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-06-15 12:12:23.000000 labeltransform2-2.1/labeltransform2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-15 12:12:23.000000 labeltransform2-2.1/labeltransform2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 12:12:23.661352 labeltransform2-2.1/setup.cfg
--rw-rw-rw-   0        0        0      436 2023-06-15 12:12:00.000000 labeltransform2-2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 11:41:55.948716 labeltransform2-2.2/
+-rw-rw-rw-   0        0        0    11558 2023-06-14 02:18:41.000000 labeltransform2-2.2/LICENSE
+-rw-rw-rw-   0        0        0      225 2023-07-01 11:41:55.926257 labeltransform2-2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      961 2023-06-14 02:18:41.000000 labeltransform2-2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-01 11:41:55.920255 labeltransform2-2.2/labeltransform2/
+-rw-rw-rw-   0        0        0       79 2023-07-01 10:02:22.000000 labeltransform2-2.2/labeltransform2/__init__.py
+-rw-rw-rw-   0        0        0      176 2023-07-01 10:00:11.000000 labeltransform2-2.2/labeltransform2/format.py
+-rw-rw-rw-   0        0        0     4537 2023-07-01 11:41:52.000000 labeltransform2-2.2/labeltransform2/generate_voc.py
+-rw-rw-rw-   0        0        0      896 2023-06-15 12:11:48.000000 labeltransform2-2.2/labeltransform2/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-01 11:41:55.926257 labeltransform2-2.2/labeltransform2/xml/
+-rw-rw-rw-   0        0        0      469 2023-06-14 03:30:14.000000 labeltransform2-2.2/labeltransform2/xml/voc.xml
+drwxrwxrwx   0        0        0        0 2023-07-01 11:41:55.925257 labeltransform2-2.2/labeltransform2.egg-info/
+-rw-rw-rw-   0        0        0      225 2023-07-01 11:41:55.000000 labeltransform2-2.2/labeltransform2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      359 2023-07-01 11:41:55.000000 labeltransform2-2.2/labeltransform2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 11:41:55.000000 labeltransform2-2.2/labeltransform2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-07-01 11:41:55.000000 labeltransform2-2.2/labeltransform2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-01 11:41:55.000000 labeltransform2-2.2/labeltransform2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-01 11:41:55.948716 labeltransform2-2.2/setup.cfg
+-rw-rw-rw-   0        0        0      436 2023-06-30 09:37:32.000000 labeltransform2-2.2/setup.py
```

### Comparing `labeltransform2-2.1/LICENSE` & `labeltransform2-2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `labeltransform2-2.1/README.md` & `labeltransform2-2.2/README.md`

 * *Files identical despite different names*

### Comparing `labeltransform2-2.1/labeltransform2/generate_voc.py` & `labeltransform2-2.2/labeltransform2/generate_voc.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,27 +3,30 @@
 from xml.etree import ElementTree as ET
 from multiprocessing import Process
 import pandas as pd
 from copy import deepcopy
 import cv2
 import pkg_resources
 
+from .format import *
+
 
 class VocStyle:
     def __init__(self, img_dir, data: Optional[pd.DataFrame]) -> None:
         self.img_dir = Path(img_dir)
         if data is not None:
             self.data = data
             self.data.columns = ["name", "cls", "x1", "y1", "x2", "y2"]
             self.names = list(set(self.data["name"].to_list()))
         else:
-            self.names = [i.stem for i in self.img_dir.glob("*.jpg") \
-                if self.img_dir.joinpath(i.stem + ".xml").exists()]
+            # TODO 这里改的不好
+            self.names = [i.stem for i in self.img_dir.glob("*") \
+            if self.img_dir.joinpath(i.stem + ".xml").exists \
+                and i.suffix[1:] in IMG_FORMATS]
         self.cls_names = {}
-    
 
     def write(self, names):
         for name in names:
             tree, root, filename, width, height, depth, obj = self.style()
             img = self.img_dir.joinpath(name + ".jpg")
             filename.text = img.name
             cv_img = cv2.imread(img.__str__())
@@ -65,16 +68,14 @@
         ymin = bndbox.find("ymin")
         xmax = bndbox.find("xmax")
         ymax = bndbox.find("ymax")
         name.text, xmin.text, ymin.text, xmax.text, ymax.text = bbox[1:]
         return obj
 
     def voc_2_yolo(self):
-        self.names = list(set(self.names) & set([i.stem for i in self.img_dir.glob("*.jpg") if \
-            self.img_dir.joinpath(i.stem + ".xml").exists()]))
         assert len(self.names) > 0
         n = len(self.names) // 5
         name_list = [self.names[i*n:(i+1)*n if i<4 else -1] for i in range(5)]
         for names in name_list:
             task = Process(target=self.voc_2_yolo_, args=(names, ))
             task.start()
 
@@ -95,31 +96,29 @@
         bboxes = []
 
         for obj in objs:
             cls = obj.find("name").text
             if cls in self.cls_names:
                 cls = self.cls_names[cls]
             else:
-                self.cls_names[cls] = len(self.cls_names)
-                cls = self.cls_names[cls]
+                continue
             bndbox = obj.find("bndbox")
             x1 = int(eval(bndbox.find("xmin").text))
             y1 = int(eval(bndbox.find("ymin").text))
             x2 = int(eval(bndbox.find("xmax").text))
             y2 = int(eval(bndbox.find("ymax").text))
             cx = (x1 + x2) / 2
             cy = (y1 + y2) / 2
             w = x2 - x1
             h = y2 - y1
             bbox = [cx / width, cy / height, w / width, h / height]
             bbox = f"{cls} " + " ".join(list(map(lambda x: str(x), bbox))) + "\n"
             bboxes.append(bbox)
-        
         return bboxes
 
 
 if __name__ == "__main__":
-    
-    names = list(range(1989))
-    n = len(names) // 5
-    name_list = [names[i*n:(i+1)*n if i<4 else -1] for i in range(5)]
-    print([len(i) for i in name_list])
+    ...
+    # names = list(range(1989))
+    # n = len(names) // 5
+    # name_list = [names[i*n:(i+1)*n if i<4 else -1] for i in range(5)]
+    # print([len(i) for i in name_list])
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `labeltransform2-2.1/labeltransform2/tools.py` & `labeltransform2-2.2/labeltransform2/tools.py`

 * *Files identical despite different names*

