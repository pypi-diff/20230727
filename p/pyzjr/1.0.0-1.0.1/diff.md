# Comparing `tmp/pyzjr-1.0.0.tar.gz` & `tmp/pyzjr-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyzjr-1.0.0.tar", last modified: Tue Jul 25 03:00:20 2023, max compression
+gzip compressed data, was "dist\pyzjr-1.0.1.tar", last modified: Thu Jul 27 10:31:55 2023, max compression
```

## Comparing `pyzjr-1.0.0.tar` & `pyzjr-1.0.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 03:00:20.000000 pyzjr-1.0.0/
--rw-rw-rw-   0        0        0     2733 2023-07-25 03:00:20.000000 pyzjr-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1547 2023-07-25 03:00:07.000000 pyzjr-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 03:00:20.000000 pyzjr-1.0.0/pyzjr/
--rw-rw-rw-   0        0        0     3959 2023-07-02 08:05:46.000000 pyzjr-1.0.0/pyzjr/ColorModule.py
--rw-rw-rw-   0        0        0    17203 2023-07-11 01:30:30.000000 pyzjr-1.0.0/pyzjr/Enimage.py
--rw-rw-rw-   0        0        0     3932 2023-07-21 17:30:08.000000 pyzjr-1.0.0/pyzjr/FM.py
--rw-rw-rw-   0        0        0     9085 2023-07-15 12:01:54.000000 pyzjr-1.0.0/pyzjr/MinIO.py
--rw-rw-rw-   0        0        0     6343 2023-07-15 12:04:40.000000 pyzjr-1.0.0/pyzjr/PIC.py
--rw-rw-rw-   0        0        0     6361 2023-07-16 03:00:08.000000 pyzjr-1.0.0/pyzjr/Showimage.py
--rw-rw-rw-   0        0        0     4544 2023-07-04 09:36:13.000000 pyzjr-1.0.0/pyzjr/TrackBar.py
--rw-rw-rw-   0        0        0      312 2023-07-12 11:15:25.000000 pyzjr-1.0.0/pyzjr/Z.py
--rw-rw-rw-   0        0        0      976 2023-07-25 03:00:09.000000 pyzjr-1.0.0/pyzjr/__init__.py
--rw-rw-rw-   0        0        0     6164 2023-07-22 02:13:00.000000 pyzjr-1.0.0/pyzjr/definition.py
--rw-rw-rw-   0        0        0     2356 2023-07-16 02:19:11.000000 pyzjr-1.0.0/pyzjr/utils.py
--rw-rw-rw-   0        0        0     4832 2023-07-24 15:58:50.000000 pyzjr-1.0.0/pyzjr/video.py
--rw-rw-rw-   0        0        0     2786 2023-07-24 16:00:54.000000 pyzjr-1.0.0/pyzjr/zmath.py
-drwxrwxrwx   0        0        0        0 2023-07-25 03:00:20.000000 pyzjr-1.0.0/pyzjr.egg-info/
--rw-rw-rw-   0        0        0     2733 2023-07-25 03:00:20.000000 pyzjr-1.0.0/pyzjr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      371 2023-07-25 03:00:20.000000 pyzjr-1.0.0/pyzjr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 03:00:20.000000 pyzjr-1.0.0/pyzjr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       85 2023-07-25 03:00:20.000000 pyzjr-1.0.0/pyzjr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-25 03:00:20.000000 pyzjr-1.0.0/pyzjr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 03:00:20.000000 pyzjr-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     2020 2023-07-25 03:00:08.000000 pyzjr-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 10:31:55.000000 pyzjr-1.0.1/
+-rw-rw-rw-   0        0        0     2838 2023-07-27 10:31:55.000000 pyzjr-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1634 2023-07-27 10:30:52.000000 pyzjr-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 10:31:55.000000 pyzjr-1.0.1/pyzjr/
+-rw-rw-rw-   0        0        0     3959 2023-07-02 08:05:46.000000 pyzjr-1.0.1/pyzjr/ColorModule.py
+-rw-rw-rw-   0        0        0    17203 2023-07-11 01:30:30.000000 pyzjr-1.0.1/pyzjr/Enimage.py
+-rw-rw-rw-   0        0        0     3932 2023-07-21 17:30:08.000000 pyzjr-1.0.1/pyzjr/FM.py
+-rw-rw-rw-   0        0        0     9085 2023-07-15 12:01:54.000000 pyzjr-1.0.1/pyzjr/MinIO.py
+-rw-rw-rw-   0        0        0     7019 2023-07-26 16:37:00.000000 pyzjr-1.0.1/pyzjr/PIC.py
+-rw-rw-rw-   0        0        0     6505 2023-07-26 16:48:15.000000 pyzjr-1.0.1/pyzjr/Showimage.py
+-rw-rw-rw-   0        0        0     4544 2023-07-04 09:36:13.000000 pyzjr-1.0.1/pyzjr/TrackBar.py
+-rw-rw-rw-   0        0        0      312 2023-07-12 11:15:25.000000 pyzjr-1.0.1/pyzjr/Z.py
+-rw-rw-rw-   0        0        0      976 2023-07-27 10:31:48.000000 pyzjr-1.0.1/pyzjr/__init__.py
+-rw-rw-rw-   0        0        0     6164 2023-07-22 02:13:00.000000 pyzjr-1.0.1/pyzjr/definition.py
+-rw-rw-rw-   0        0        0     2356 2023-07-16 02:19:11.000000 pyzjr-1.0.1/pyzjr/utils.py
+-rw-rw-rw-   0        0        0     4832 2023-07-24 15:58:50.000000 pyzjr-1.0.1/pyzjr/video.py
+-rw-rw-rw-   0        0        0     3637 2023-07-27 04:09:54.000000 pyzjr-1.0.1/pyzjr/zmath.py
+drwxrwxrwx   0        0        0        0 2023-07-27 10:31:55.000000 pyzjr-1.0.1/pyzjr.egg-info/
+-rw-rw-rw-   0        0        0     2838 2023-07-27 10:31:55.000000 pyzjr-1.0.1/pyzjr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2023-07-27 10:31:55.000000 pyzjr-1.0.1/pyzjr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 10:31:55.000000 pyzjr-1.0.1/pyzjr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       97 2023-07-27 10:31:55.000000 pyzjr-1.0.1/pyzjr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-27 10:31:55.000000 pyzjr-1.0.1/pyzjr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 10:31:55.000000 pyzjr-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     2044 2023-07-27 10:31:46.000000 pyzjr-1.0.1/setup.py
```

### Comparing `pyzjr-1.0.0/PKG-INFO` & `pyzjr-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyzjr
-Version: 1.0.0
+Version: 1.0.1
 Summary:  A computer vision library that supports Win, packaged with patches for visual libraries such as                 Opencv, matplotlib, and image. In the future, Pytorch will also be supported, all of which are personal (Auorui)                 engineering code experience. 
 Home-page: https://github.com/Auorui/pyzjr
 Author: Auorui
 Author-email: zjricetea@gmail.com
 License: MIT
 Description: 
         # pyzjr
@@ -25,14 +25,16 @@
         ## Installation
         
         https://pypi.org/project/pyzjr/
         
         https://github.com/Auorui/pyzjr (I want stars ⭐ hhh)
         
         ## Update log
+        `1.0.1` Modified the issue of incorrect color in the stacked display of torch images.
+        
         `1.0.0` Official upload of version 1.0.0
         
         `0.0.19` Modified the problem of Escape character in the path read by the getPhotopath function
         
         `0.0.17——0.018` Added Showimage module and added torch framework. It is recommended to install it in a virtual environment of deep learning framework.
         
         `0.0.12——0.016` Modifying bugs and adding functions to the PIC.py file.
```

### Comparing `pyzjr-1.0.0/README.md` & `pyzjr-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 ## Installation
 
 https://pypi.org/project/pyzjr/
 
 https://github.com/Auorui/pyzjr (I want stars ⭐ hhh)
 
 ## Update log
+`1.0.1` Modified the issue of incorrect color in the stacked display of torch images.
+
 `1.0.0` Official upload of version 1.0.0
 
 `0.0.19` Modified the problem of Escape character in the path read by the getPhotopath function
 
 `0.0.17——0.018` Added Showimage module and added torch framework. It is recommended to install it in a virtual environment of deep learning framework.
 
 `0.0.12——0.016` Modifying bugs and adding functions to the PIC.py file.
```

### Comparing `pyzjr-1.0.0/pyzjr/ColorModule.py` & `pyzjr-1.0.1/pyzjr/ColorModule.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.0.0/pyzjr/Enimage.py` & `pyzjr-1.0.1/pyzjr/Enimage.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.0.0/pyzjr/FM.py` & `pyzjr-1.0.1/pyzjr/FM.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.0.0/pyzjr/MinIO.py` & `pyzjr-1.0.1/pyzjr/MinIO.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.0.0/pyzjr/PIC.py` & `pyzjr-1.0.1/pyzjr/PIC.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 import pyzjr.Z as Z
 
 from skimage.morphology import skeletonize
 from skimage.filters import threshold_otsu
 from skimage.color import rgb2gray
 from skimage import measure
 
+import torch
+from torchvision import transforms
+
 def repairImg(img,r=5,flags=Z.repair_NS,mode=0):
     """
     * 用于修复图像
     :param img: 输入图像
     :param r: 修复半径，即掩膜的像素周围需要参考的区域半径
     :param flags: 修复算法的标志,有Z.repair_NS、Z.repair_TELEA,默认为Z.repair_NS
     :param mode: 是否采用HSV例模式,默认为0,自定义模式,可通过Color下的TrackBar文件中获得
@@ -144,7 +147,30 @@
     """
     binary_image = BinaryImg(img)
     contours = measure.find_contours(binary_image, level=128, fully_connected='low', positive_orientation='low')
     contour_coordinates = []
     for contour in contours:
         contour_coordinates.extend([(int(coord[1]), int(coord[0])) for coord in contour])
     return contour_coordinates
+
+
+def cvtColor(image):
+    """转化为RGB格式"""
+    if len(np.shape(image)) == 3 and np.shape(image)[2] == 3:
+        return image
+    else:
+        img = image.convert('RGB')
+        return img
+
+def imtensor(image):
+    """转化为tensor格式
+    image1 = Image.open(path).convert('L')
+    image2 = pz.imtensor(image1)
+    """
+    preprocess = transforms.ToTensor()
+    image_tensor = preprocess(image).unsqueeze(0)
+    return image_tensor
+
+def impillow(input_tensor):
+    """将tensor再转化为PIL"""
+    output_image = transforms.ToPILImage()(input_tensor.squeeze(0))
+    return output_image
```

### Comparing `pyzjr-1.0.0/pyzjr/Showimage.py` & `pyzjr-1.0.1/pyzjr/Showimage.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,40 +95,44 @@
         stacked_image[y:y+image_height, x:x+image_width, :] = image
 
     plt.imshow(stacked_image)
     plt.axis('off')  # 关闭坐标轴显示
     plt.show()
 
 
-def Stackedtorch(imgs, num_rows, num_cols, titles=None, scale=1.5):
+def Stackedtorch(imgs, num_rows, num_cols, titles=None, scale=None, camp=None):
     """
     堆叠显示Tensor图像或PIL图像
     :param imgs: 包含图像的列表,可以包含Tensor图像或PIL图像
     :param num_rows: 图像的行数
     :param num_cols: 图像的列数
     :param titles: 图像的标题列表,默认为None
-    :param scale: 图像的缩放比例,默认为1.5
+    :param scale: 图像的缩放比例,默认为None
+    :param camp: 'gray'
     :return:
     example:
         imgs = [image1, image2, image3, image4]
         titles = ['Image 1', 'Image 2', 'Image 3','Image 4']
         axes = Stackedtorch(imgs, 2, 2, titles=titles, scale=5)
         plt.savefig('my_plot.jpg')
         plt.show()
     """
-    figsize = (num_cols * scale, num_rows * scale)
-    _, axes = plt.subplots(num_rows, num_cols, figsize=figsize)
+    if scale:
+        figsize = (num_cols * scale, num_rows * scale)
+        _, axes = plt.subplots(num_rows, num_cols, figsize=figsize)
+    else:
+        _, axes = plt.subplots(num_rows, num_cols)
     axes = axes.flatten()
     for i, (ax, img) in enumerate(zip(axes, imgs)):
         if torch.is_tensor(img):
             # Tensor Image
-            ax.imshow(img.numpy())
+            ax.imshow(img.numpy(),cmap=camp)
         else:
             # PIL Image
-            ax.imshow(img)
+            ax.imshow(img,cmap=camp)
         ax.axes.get_xaxis().set_visible(False)
         ax.axes.get_yaxis().set_visible(False)
         if titles:
             ax.set_title(titles[i])
     return axes
 
 def plot_line(x, y, xlabel, ylabel, title):
```

### Comparing `pyzjr-1.0.0/pyzjr/TrackBar.py` & `pyzjr-1.0.1/pyzjr/TrackBar.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.0.0/pyzjr/__init__.py` & `pyzjr-1.0.1/pyzjr/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
   At present, it is only for my personal use. If you want to
   use it, please contact me. Here are my email and WeChat.
 - WeChat: z15583909992
 - Email: zjricetea@gmail.com
 - Note: Currently still being updated, please refer to the latest version for any changes that may occur
 """
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 
 import cv2
 
 from pyzjr.Enimage import Filter,Enhance,Random_Enhance,Retinex
 from pyzjr.definition import *
 from pyzjr.ColorModule import *
 from pyzjr.definition import *
```

### Comparing `pyzjr-1.0.0/pyzjr/definition.py` & `pyzjr-1.0.1/pyzjr/definition.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.0.0/pyzjr/utils.py` & `pyzjr-1.0.1/pyzjr/utils.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.0.0/pyzjr/video.py` & `pyzjr-1.0.1/pyzjr/video.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.0.0/pyzjr/zmath.py` & `pyzjr-1.0.1/pyzjr/zmath.py`

 * *Files 27% similar despite different names*

```diff
@@ -18,79 +18,91 @@
     return round(value,t)
 
 def normal(x, mu, sigma):
     """正态分布（高斯分布）概率密度函数"""
     p = 1 / np.sqrt(2 * np.pi * sigma**2)
     return p * np.exp(-0.5 / sigma**2 * (x - mu)**2)
 
+def Advancedlist(imglist,mode='T',reverse=False):
+    """对列表的高级排列"""
+    if mode=="T":
+        """平铺
+        lists = [[1, 2, 3], [4, 5, 6], [7, 8, 9]] ——> [1, 2, 3, 4, 5, 6, 7, 8, 9]
+        """
+        tiled_list = [item for sublist in imglist for item in sublist]
+        return tiled_list
+    elif mode=="F":
+        """首元素
+        lists = [[1, 2, 3], [4, 5, 6], [7, 8, 9]] ——> [1, 4, 7, 2, 5, 8, 3, 6, 9]
+        """
+        sorted_list_by_first_element = [sublist[i] for i in range(len(imglist[0])) for sublist in imglist]
+        return sorted_list_by_first_element
+    elif mode=="X":
+        """按照x排序,默认是从小到大
+        lists = [(1, 4), (3, 8), (5, 2)] ——> [(1, 4), (3, 8), (5, 2)]
+        """
+        sorted_by_x = sorted(imglist, key=lambda item: item[0], reverse=reverse)
+        return sorted_by_x
+    elif mode=="Y":
+        """按照y排序,默认是从小到大
+        lists = [(1, 4), (3, 8), (5, 2)] ——> [(5, 2), (1, 4), (3, 8)]
+        """
+        sorted_by_y = sorted(imglist, key=lambda item: item[1], reverse=reverse)
+        return sorted_by_y
+
+
 class pysort():
     def insertion_sort(self, arr):
         """
         直接插入排序
-        :param arr:
-        :return:
         """
         n = len(arr)
         for i in range(1, n):
             key = arr[i]
             j = i - 1
             while j >= 0 and arr[j] > key:
                 arr[j + 1] = arr[j]
                 j -= 1
             arr[j + 1] = key
             print(arr)
 
     def quick_sort(self, arr, low, high):
         """
         快速排序
-        :param arr:
-        :param low:
-        :param high:
-        :return:
         """
         if low < high:
             pivot_index = self.partition(arr, low, high)
             print(arr)
             self.quick_sort(arr, low, pivot_index - 1)
             self.quick_sort(arr, pivot_index + 1, high)
 
     def partition(self, arr, low, high):
-        """
-        :param arr:
-        :param low:
-        :param high:
-        :return:
-        """
         pivot = arr[high]
         i = low - 1
         for j in range(low, high):
             if arr[j] <= pivot:
                 i += 1
                 arr[i], arr[j] = arr[j], arr[i]
         arr[i + 1], arr[high] = arr[high], arr[i + 1]
         return i + 1
 
     def bubble_sort(self, arr):
         """
         冒泡排序
-        :param arr:
-        :return:
         """
         n = len(arr)
         for i in range(n - 1):
             for j in range(n - 1 - i):
                 if arr[j] > arr[j + 1]:
                     arr[j], arr[j + 1] = arr[j + 1], arr[j]
             print(arr)
 
     def selection_sort(self, arr):
         """
         直接选择排序
-        :param arr:
-        :return:
         """
         n = len(arr)
         for i in range(n - 1):
             min_index = i
             for j in range(i + 1, n):
                 if arr[j] < arr[min_index]:
                     min_index = j
```

### Comparing `pyzjr-1.0.0/pyzjr.egg-info/PKG-INFO` & `pyzjr-1.0.1/pyzjr.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyzjr
-Version: 1.0.0
+Version: 1.0.1
 Summary:  A computer vision library that supports Win, packaged with patches for visual libraries such as                 Opencv, matplotlib, and image. In the future, Pytorch will also be supported, all of which are personal (Auorui)                 engineering code experience. 
 Home-page: https://github.com/Auorui/pyzjr
 Author: Auorui
 Author-email: zjricetea@gmail.com
 License: MIT
 Description: 
         # pyzjr
@@ -25,14 +25,16 @@
         ## Installation
         
         https://pypi.org/project/pyzjr/
         
         https://github.com/Auorui/pyzjr (I want stars ⭐ hhh)
         
         ## Update log
+        `1.0.1` Modified the issue of incorrect color in the stacked display of torch images.
+        
         `1.0.0` Official upload of version 1.0.0
         
         `0.0.19` Modified the problem of Escape character in the path read by the getPhotopath function
         
         `0.0.17——0.018` Added Showimage module and added torch framework. It is recommended to install it in a virtual environment of deep learning framework.
         
         `0.0.12——0.016` Modifying bugs and adding functions to the PIC.py file.
```

### Comparing `pyzjr-1.0.0/setup.py` & `pyzjr-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # these things are needed for the README.md show on pypi (if you dont need delete it)
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 
-VERSION = '1.0.0'
+VERSION = '1.0.1'
 DESCRIPTION = ' A computer vision library that supports Win, packaged with patches for visual libraries such as \
                 Opencv, matplotlib, and image. In the future, Pytorch will also be supported, all of which are personal (Auorui) \
                 engineering code experience. '
 LONG_DESCRIPTION = 'pyzjr is a computer vision library that supports Win'
 
 setup(
     name="pyzjr",
@@ -43,15 +43,16 @@
         'matplotlib',
         'numpy',
         'imageio',
         'scikit-image',
         'torch',
         'opencv-python',
         'pillow',
-        'minio'
+        'minio',
+        'torchvision'
     ],
     keywords=['python', 'computer vision', 'pyzjr','windows'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Microsoft :: Windows",
```

