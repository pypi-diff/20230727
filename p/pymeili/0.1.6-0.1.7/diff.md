# Comparing `tmp/pymeili-0.1.6.tar.gz` & `tmp/pymeili-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymeili-0.1.6.tar", last modified: Thu Jul 27 10:00:28 2023, max compression
+gzip compressed data, was "pymeili-0.1.7.tar", last modified: Thu Jul 27 15:38:59 2023, max compression
```

## Comparing `pymeili-0.1.6.tar` & `pymeili-0.1.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 10:00:28.242092 pymeili-0.1.6/
--rw-rw-rw-   0        0        0      384 2023-07-27 09:58:37.000000 pymeili-0.1.6/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1057 2023-07-25 12:28:38.000000 pymeili-0.1.6/LISCENCE.txt
--rw-rw-rw-   0        0        0       36 2023-07-25 15:28:50.000000 pymeili-0.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0     1550 2023-07-27 10:00:28.242092 pymeili-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      714 2023-07-26 14:23:15.000000 pymeili-0.1.6/README.txt
-drwxrwxrwx   0        0        0        0 2023-07-27 10:00:28.211522 pymeili-0.1.6/pymeili/
-drwxrwxrwx   0        0        0        0 2023-07-27 10:00:28.240590 pymeili-0.1.6/pymeili/FONT/
--rw-rw-rw-   0        0        0    40028 2016-07-20 20:40:52.000000 pymeili-0.1.6/pymeili/FONT/Futura Extra Black font.ttf
--rw-rw-rw-   0        0        0    38980 2016-07-20 20:40:52.000000 pymeili-0.1.6/pymeili/FONT/Futura Heavy font.ttf
--rw-rw-rw-   0        0        0    38764 2016-07-20 20:40:54.000000 pymeili-0.1.6/pymeili/FONT/futura medium bt.ttf
--rw-rw-rw-   0        0        0      785 2023-07-27 09:58:43.000000 pymeili-0.1.6/pymeili/__init__.py
--rw-rw-rw-   0        0        0    57797 2023-07-27 09:57:48.000000 pymeili-0.1.6/pymeili/beautifyplot.py
-drwxrwxrwx   0        0        0        0 2023-07-27 10:00:28.225074 pymeili-0.1.6/pymeili.egg-info/
--rw-rw-rw-   0        0        0     1550 2023-07-27 10:00:28.000000 pymeili-0.1.6/pymeili.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      336 2023-07-27 10:00:28.000000 pymeili-0.1.6/pymeili.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 10:00:28.000000 pymeili-0.1.6/pymeili.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-27 10:00:28.000000 pymeili-0.1.6/pymeili.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 10:00:28.242092 pymeili-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      741 2023-07-27 09:58:47.000000 pymeili-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 15:38:59.843371 pymeili-0.1.7/
+-rw-rw-rw-   0        0        0      433 2023-07-27 13:09:18.000000 pymeili-0.1.7/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1057 2023-07-25 12:28:38.000000 pymeili-0.1.7/LISCENCE.txt
+-rw-rw-rw-   0        0        0       36 2023-07-25 15:28:50.000000 pymeili-0.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     1627 2023-07-27 15:38:59.843371 pymeili-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      742 2023-07-27 13:10:18.000000 pymeili-0.1.7/README.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 15:38:59.813415 pymeili-0.1.7/pymeili/
+drwxrwxrwx   0        0        0        0 2023-07-27 15:38:59.841376 pymeili-0.1.7/pymeili/FONT/
+-rw-rw-rw-   0        0        0    40028 2016-07-20 20:40:52.000000 pymeili-0.1.7/pymeili/FONT/Futura Extra Black font.ttf
+-rw-rw-rw-   0        0        0    38980 2016-07-20 20:40:52.000000 pymeili-0.1.7/pymeili/FONT/Futura Heavy font.ttf
+-rw-rw-rw-   0        0        0    38764 2016-07-20 20:40:54.000000 pymeili-0.1.7/pymeili/FONT/futura medium bt.ttf
+-rw-rw-rw-   0        0        0      785 2023-07-27 13:08:56.000000 pymeili-0.1.7/pymeili/__init__.py
+-rw-rw-rw-   0        0        0    60827 2023-07-27 15:38:43.000000 pymeili-0.1.7/pymeili/beautifyplot.py
+drwxrwxrwx   0        0        0        0 2023-07-27 15:38:59.828442 pymeili-0.1.7/pymeili.egg-info/
+-rw-rw-rw-   0        0        0     1627 2023-07-27 15:38:59.000000 pymeili-0.1.7/pymeili.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      336 2023-07-27 15:38:59.000000 pymeili-0.1.7/pymeili.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 15:38:59.000000 pymeili-0.1.7/pymeili.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-27 15:38:59.000000 pymeili-0.1.7/pymeili.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 15:38:59.843371 pymeili-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      741 2023-07-27 13:09:50.000000 pymeili-0.1.7/setup.py
```

### Comparing `pymeili-0.1.6/LISCENCE.txt` & `pymeili-0.1.7/LISCENCE.txt`

 * *Files identical despite different names*

### Comparing `pymeili-0.1.6/PKG-INFO` & `pymeili-0.1.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: pymeili
-Version: 0.1.6
+Version: 0.1.7
 Summary: a module to beautify your python plot.
 Home-page: 
 Author: VVVictorZhou
 Author-email: vichouro@gmail.com
 License: MIT
 Keywords: beautify
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 
-pymeili is a module to beautify your python plot with more simple way. the design idea is from Navigraph aeronautical chart.
+【pymeli.為美麗而生】pymeili is a module to beautify your python plot with more simple way. the design idea is from Navigraph aeronautical chart.
 
 【IMPORTANT】
 Before using this module, you need to install font-packages: https://dwl.freefontsfamily.com/download/futura/; moving the font file to installed module folder(e.g. C:\Users\Username\AppData\Local\Programs\Python\Python311\Lib\site-packages\pymeili).
-For more information and instruction, please go to https://github.com/VVVICTORZHOU/resources.git; or you can just download the font file from the link above.
+For more information and instruction, please go to: https://github.com/VVVICTORZHOU/resources.git or you can just download the font file from the link above.
 
 
 Install guide: (run on your powershell or cmd)
 > pip install pymeili
 
 Update guide: (run on your powershell or cmd)
 > pip install --upgrade pymeili
@@ -47,7 +47,10 @@
 - Fix Some Minor Problems
 
 0.1.5 (27/07/2023)
 - Add Basic Basemap Function, fix some problems
 
 0.1.6 (27/07/2023)
 - Fix Some Problems, add common raise function
+
+0.1.7 (27/07/2023)
+- Fix Some Minor Problems
```

### Comparing `pymeili-0.1.6/README.txt` & `pymeili-0.1.7/README.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-pymeili is a module to beautify your python plot with more simple way. the design idea is from Navigraph aeronautical chart.
+【pymeli.為美麗而生】pymeili is a module to beautify your python plot with more simple way. the design idea is from Navigraph aeronautical chart.
 
 【IMPORTANT】
 Before using this module, you need to install font-packages: https://dwl.freefontsfamily.com/download/futura/; moving the font file to installed module folder(e.g. C:\Users\Username\AppData\Local\Programs\Python\Python311\Lib\site-packages\pymeili).
-For more information and instruction, please go to https://github.com/VVVICTORZHOU/resources.git; or you can just download the font file from the link above.
+For more information and instruction, please go to: https://github.com/VVVICTORZHOU/resources.git or you can just download the font file from the link above.
 
 
 Install guide: (run on your powershell or cmd)
 > pip install pymeili
 
 Update guide: (run on your powershell or cmd)
 > pip install --upgrade pymeili
```

### Comparing `pymeili-0.1.6/pymeili/FONT/Futura Extra Black font.ttf` & `pymeili-0.1.7/pymeili/FONT/Futura Extra Black font.ttf`

 * *Files identical despite different names*

### Comparing `pymeili-0.1.6/pymeili/FONT/Futura Heavy font.ttf` & `pymeili-0.1.7/pymeili/FONT/Futura Heavy font.ttf`

 * *Files identical despite different names*

### Comparing `pymeili-0.1.6/pymeili/FONT/futura medium bt.ttf` & `pymeili-0.1.7/pymeili/FONT/futura medium bt.ttf`

 * *Files identical despite different names*

### Comparing `pymeili-0.1.6/pymeili/__init__.py` & `pymeili-0.1.7/pymeili/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,8 +20,8 @@
     fill_between, fill_betweenx,
     pause, normalize, adjust, addaxes, slider, set_xydata,
     figsize, show, clf, close, figure, savefig,
     imread, imshow, imsave,
     
 )
 
-__version__: str = '0.1.6'
+__version__: str = '0.1.7'
```

### Comparing `pymeili-0.1.6/pymeili/beautifyplot.py` & `pymeili-0.1.7/pymeili/beautifyplot.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,22 @@
 # 刪去__file__中最後面自"\"開始的字串(刪除檔名)
 motherpath = currentfilepath[:-len(currentfilepath.split('\\')[-1])]
 try:
     fontpath = Path(mpl.get_data_path(), motherpath+"\\futura medium bt.ttf")
     fontpath_bold = Path(mpl.get_data_path(), motherpath+"\Futura Heavy font.ttf")
     fontpath_black = Path(mpl.get_data_path(), motherpath+"\Futura Extra Black font.ttf")
 except: # 未安裝字體
-    raise Exception(bcolors.WARNING+'Please install Futura fonts in the same directory as this file.\ninstall font-packages: https://dwl.freefontsfamily.com/download/futura/;\n Moving the font file to installed module folder(e.g."C:>Users>Username>AppData>Local>Programs>Python>Python311>Lib>site-packages>pymeili").'+bcolors.ENDC)
+    try:
+        # 退而求其次，使用預設字體
+        fontpath = 'C:\Windows\Fonts\Arial.ttf'
+        fontpath_bold = 'C:\Windows\Fonts\Arial Bold.ttf'
+        fontpath_black = 'C:\Windows\Fonts\Arial Black.ttf'
+        print(bcolors.WARNING+'Please install Futura fonts in the same directory as this file.\ninstall font-packages: https://dwl.freefontsfamily.com/download/futura/;\n Moving the font file to installed module folder(e.g."C:>Users>Username>AppData>Local>Programs>Python>Python311>Lib>site-packages>pymeili").\n Currently using system default font: Arial'+bcolors.ENDC)
+    except:
+        raise Exception(bcolors.WARNING+'Please install Futura fonts in the same directory as this file.\ninstall font-packages: https://dwl.freefontsfamily.com/download/futura/;\n Moving the font file to installed module folder(e.g."C:>Users>Username>AppData>Local>Programs>Python>Python311>Lib>site-packages>pymeili").'+bcolors.ENDC)
 '''
 # METHOD II
 url_medium = r'https://github.com/VVVICTORZHOU/resources/blob/main/futura%20medium%20bt.ttf'
 url_Heavy = r'https://github.com/VVVICTORZHOU/resources/blob/main/Futura%20Heavy%20font.ttf'
 url_Black = r'https://github.com/VVVICTORZHOU/resources/blob/main/Futura%20Extra%20Black%20font.ttf'
 
 fontpath = Path(mpl.get_data_path(), urllib3.PoolManager().request('GET', url_medium).data)
@@ -288,38 +295,69 @@
 def polar(theta, r, color='fg', linewidth=2, linestyle='-', label=getPLOTNO(),**kwargs):
     plt.polar(theta, r, color=colorlist(color), linewidth=linewidth, label=label,linestyle=linestyle, **kwargs)
 
 # contour繪圖
 def contour(x, y, z, colors='fg', levels=10, linewidths=2, clabel=True, fontsize=12, color='fg', **kwargs):
     CS = plt.contour(x, y, z, colors=colorlist(colors), levels=levels, linewidths=linewidths, **kwargs)
     if clabel == True:
-        CL = CS.clabel(fontsize=fontsize, colors=colorlist(color), inline=True)
+        CL = CS.clabel(fontsize=fontsize, colors=colorlist(color), inline=True, levels=levels, **kwargs)
+
 
 # contourf繪圖
-def contourf(x, y, z, levels=10, cmap='28', contour=True, clabel=True,linewidths=1.5, color='fg', **kwargs):
+def contourf(x, y, z, levels=10, cmap='28', contour=True, clabel=True,linewidths=1.5, color='fg', vmin='auto', vmax='auto',**kwargs):
+    import numpy as np
+    # 傳出Z值和levels值
+    global contour_vmin, contour_vmax, contour_levels
+    contour_levels = levels
+    if vmin == 'auto':
+        vmin = np.floor(z.min()/10**(len(str(int(z.min())))-2))*10**(len(str(int(z.min())))-2)
+        contour_vmin = vmin
+    else:
+        contour_vmin = vmin
+    if vmax == 'auto':
+        vmax = np.ceil(z.max()/10**(len(str(int(z.max())))-2))*10**(len(str(int(z.max())))-2)
+        contour_vmax = vmax
+    else:
+        contour_vmax = vmax
+    
     if contour == True:
         CS = plt.contour(x, y, z, colors=colorlist(color), levels=levels, linewidths=linewidths)
     if clabel == True:
         CL = CS.clabel(fontsize=8, colors=colorlist(color), inline=True)
-    plt.contourf(x, y, z, cmap=cmaplist(cmap), **kwargs)
+    plt.contourf(x, y, z, cmap=cmaplist(cmap), vmin=vmin, vmax=vmax, levels=levels, **kwargs)
+
+
 
 # colorbar顯示
-def colorbar(ticks,label=' ', orientation='vertical',shrink=0.95, aspect=20, fraction=0.046, pad=0.04, labelfontsize=16, font=fontpath, color='fg',**kwargs):
+def colorbar(ticks='auto',label=' ', orientation='vertical',shrink=0.95, aspect=20, fraction=0.046, pad=0.04, labelfontsize=16, font=fontpath, color='fg', extebd='neither',**kwargs):
     if orientation == 'v' or 'V':
         orientation = 'vertical'
     elif orientation == 'h' or 'H':
         orientation = 'horizontal'
-    CB = plt.colorbar(orientation=orientation, shrink=shrink, aspect=aspect, label=label, fraction=fraction, pad=pad, **kwargs)
+    if ticks == 'auto':
+        import numpy as np
+        ticks = []
+        for i in range(contour_levels):
+            ticks.append(contour_vmin+(contour_vmax-contour_vmin)/(contour_levels-1)*i)
+        extend = 'both'
+        CB = plt.colorbar(ticks=ticks, orientation=orientation, shrink=shrink, aspect=aspect, label=label, fraction=fraction, pad=pad, extend=extend, **kwargs)
+        plt.clim(contour_vmin, contour_vmax)
+        
+    else:
+        CB = plt.colorbar(ticks=ticks, orientation=orientation, shrink=shrink, aspect=aspect, label=label, fraction=fraction, pad=pad, extend=extend, **kwargs)
     CB.ax.tick_params(labelsize=labelfontsize, labelcolor=colorlist(color), color=colorlist(color))
     CB.ax.set_ylabel(label, fontproperties=fm.FontProperties(fname=font, size=labelfontsize), color=colorlist(color))
     CB.ax.set_yticks(ticks,ticks, fontproperties=fm.FontProperties(fname=font, size=labelfontsize))
     CB.ax.yaxis.set_tick_params(color=colorlist(color), labelcolor=colorlist(color))
     CB.outline.set_color(colorlist(color))
     CB.outline.set_linewidth(2)
 
+def clim(vmin, vmax):
+    plt.clim(vmin, vmax)
+
 # 直方圖
 def hist(x, bins=5, color='1', edgecolor='fg', linewidth=3, label=getHISTNO(), **kwargs):
     plt.hist(x, bins=bins, color=colorlist(color), edgecolor=colorlist(edgecolor), linewidth=linewidth, label=label,**kwargs)
 
 def hist2d(x, y, bins=5, cmap='2', **kwargs):
     plt.hist2d(x, y, bins=bins, cmap=cmaplist(cmap), **kwargs)
 
@@ -927,16 +965,32 @@
         self.ax[self.row,self.col].polar(theta, r, color=colorlist(color), linewidth=linewidth, linestyle=linestyle, **kwargs)
     
     # 繪製等值線
     def contour(self, x, y, z, colors='fg', levels=10, linewidths=2, clabel=True, fontsize=12*fontscale, color='fg', **kwargs):
         CS = self.ax[self.row,self.col].contour(x, y, z, colors=colorlist(colors), levels=levels, linewidths=linewidths, **kwargs)
         if clabel == True:
             CL = CS.clabel(fontsize=fontsize, colors=colorlist(color), inline=True)
+        self.z = z
+        self.levels = levels
     # 繪製等值線填色圖
-    def contourf(self, x, y, z, levels=10, cmap='2', contour=True, clabel=True,linewidths=1.5, color='fg', **kwargs):
+    def contourf(self, x, y, z, levels=10, cmap='2', contour=True, clabel=True,linewidths=1.5, color='fg', vmin='auto', vmax='auto', **kwargs):
+        import numpy as np
+        # 傳出Z值和levels值
+        global subcontour_vmin, subcontour_vmax, subcontour_levels
+        subcontour_levels = levels
+        if vmin == 'auto':
+            vmin = np.floor(z.min()/10**(len(str(int(z.min())))-2))*10**(len(str(int(z.min())))-2)
+            subcontour_vmin = vmin
+        else:
+            subcontour_vmin = vmin
+        if vmax == 'auto':
+            vmax = np.ceil(z.max()/10**(len(str(int(z.max())))-2))*10**(len(str(int(z.max())))-2)
+            subcontour_vmax = vmax
+        else:
+            subcontour_vmax = vmax
         if contour == True:
             CS = self.ax[self.row,self.col].contour(x, y, z, colors=colorlist(color), levels=levels, linewidths=linewidths)
         if clabel == True:
             CL = CS.clabel(fontsize=8*fontscale, colors=colorlist(color), inline=True)
         self.ax[self.row,self.col].contourf(x, y, z, cmap=cmaplist(cmap), **kwargs)
     # 繪製圖例
     def legend(self, loc='best', fontsize=18*fontscale, labelcolor='fg', frameon=True, framealpha=1, facecolor='rfg', edgecolor='fg', edgewidth=2 ,roundedge=False, **kwargs):
@@ -944,22 +998,38 @@
         if roundedge == False:
             LG.get_frame().set_boxstyle('Round', pad=0.2, rounding_size=-0.01)
         LG.get_frame().set_linewidth(edgewidth)
     # 繪製文字
     def text(self, x, y, text, color='fg', font=fontpath, fontsize=20*fontscale, **kwargs):
         self.ax[self.row,self.col].text(x, y, text, color=colorlist(color), fontproperties=fm.FontProperties(fname=font, size=fontsize), **kwargs)
     # 繪製colorbar
-    def colorbar(self, ticks,label=' ', orientation='vertical',shrink=0.95, aspect=20, labelfontsize=16*fontscale, font=fontpath, color='fg',**kwargs):
-        CB = self.ax[self.row,self.col].colorbar(orientation=orientation, shrink=shrink, aspect=aspect, label=label, **kwargs)
+    def colorbar(self, ticks='auto',label=' ', orientation='vertical',shrink=0.95, aspect=20, labelfontsize=16*fontscale, font=fontpath, extend='neither',color='fg',**kwargs):
+        if ticks == 'auto':
+            import numpy as np
+            # 獲取z,levels，並計算ticks
+            ticks = []
+            for i in range(subcontour_levels):
+                ticks.append(subcontour_vmin + (subcontour_vmax-subcontour_vmin)/subcontour_levels*i)
+            plt.clim(subcontour_vmin, subcontour_vmax)
+            extend = 'both'
+        else:
+            ticks = ticks
+        
+        
+        CB = self.ax[self.row,self.col].colorbar(orientation=orientation, shrink=shrink, aspect=aspect, label=label, extend=extend, **kwargs)
         CB.ax[self.row,self.col].tick_params(labelsize=labelfontsize, labelcolor=colorlist(color), color=colorlist(color))
         CB.ax[self.row,self.col].set_ylabel(label, fontproperties=fm.FontProperties(fname=font, size=labelfontsize), color=colorlist(color))
         CB.ax[self.row,self.col].set_yticks(ticks,ticks, fontproperties=fm.FontProperties(fname=font, size=labelfontsize))
         CB.ax[self.row,self.col].yaxis.set_tick_params(color=colorlist(color), labelcolor=colorlist(color))
         CB.outline.set_color(colorlist(color))
         CB.outline.set_linewidth(2)
+
+    def clim(self, vmin=None, vmax=None):
+        self.ax[self.row,self.col].set_clim(vmin, vmax)
+    
     # 繪製xticks、yticks
     def xticks(self, ticks, labels, color='fg', font=fontpath, fontsize=18*fontscale, **kwargs):
         self.ax[self.row,self.col].set_xticks(ticks, labels, color=colorlist(color), fontproperties=fm.FontProperties(fname=font, size=fontsize), **kwargs)
     def yticks(self, ticks, labels, color='fg', font=fontpath, fontsize=18*fontscale, **kwargs):
         self.ax[self.row,self.col].set_yticks(ticks, labels, color=colorlist(color), fontproperties=fm.FontProperties(fname=font, size=fontsize), **kwargs)
     def xlabel(self, xlabel, color='fg', font=fontpath, fontsize=24*fontscale, **kwargs):
         self.ax[self.row,self.col].set_xlabel(xlabel, color=colorlist(color), fontproperties=fm.FontProperties(fname=font, size=fontsize), **kwargs)
@@ -1044,20 +1114,15 @@
 def normalize(data, vmin=None, vmax=None):
     plt.Normalize(data, vmin=vmin, vmax=vmax)
 
 def slider(ax, label, valmin, valmax, valinit=0, valfmt='%1.2f', valstep=None, orientation='horizontal', **kwargs):
     return Slider(ax, label, valmin, valmax, valinit=valinit, valfmt=valfmt, valstep=valstep, orientation=orientation, **kwargs)
 
 
+# https://matplotlib.org/stable/gallery/widgets/slider_demo.html
 
 
 
-    
-
-
-
-# https://matplotlib.org/stable/gallery/widgets/slider_demo.html
-
 
+    
 
 
-
```

### Comparing `pymeili-0.1.6/pymeili.egg-info/PKG-INFO` & `pymeili-0.1.7/pymeili.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: pymeili
-Version: 0.1.6
+Version: 0.1.7
 Summary: a module to beautify your python plot.
 Home-page: 
 Author: VVVictorZhou
 Author-email: vichouro@gmail.com
 License: MIT
 Keywords: beautify
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 
-pymeili is a module to beautify your python plot with more simple way. the design idea is from Navigraph aeronautical chart.
+【pymeli.為美麗而生】pymeili is a module to beautify your python plot with more simple way. the design idea is from Navigraph aeronautical chart.
 
 【IMPORTANT】
 Before using this module, you need to install font-packages: https://dwl.freefontsfamily.com/download/futura/; moving the font file to installed module folder(e.g. C:\Users\Username\AppData\Local\Programs\Python\Python311\Lib\site-packages\pymeili).
-For more information and instruction, please go to https://github.com/VVVICTORZHOU/resources.git; or you can just download the font file from the link above.
+For more information and instruction, please go to: https://github.com/VVVICTORZHOU/resources.git or you can just download the font file from the link above.
 
 
 Install guide: (run on your powershell or cmd)
 > pip install pymeili
 
 Update guide: (run on your powershell or cmd)
 > pip install --upgrade pymeili
@@ -47,7 +47,10 @@
 - Fix Some Minor Problems
 
 0.1.5 (27/07/2023)
 - Add Basic Basemap Function, fix some problems
 
 0.1.6 (27/07/2023)
 - Fix Some Problems, add common raise function
+
+0.1.7 (27/07/2023)
+- Fix Some Minor Problems
```

### Comparing `pymeili-0.1.6/setup.py` & `pymeili-0.1.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: OS Independent',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='pymeili',
-    version='0.1.6',
+    version='0.1.7',
     description='a module to beautify your python plot.',
     long_description=open('README.txt',encoding="utf-8").read() + '\n\n' + open('CHANGELOG.txt',encoding="utf-8").read(),
     url='',
     author='VVVictorZhou',
     author_email='vichouro@gmail.com',
     license='MIT',
     classifiers=classifiers,
```

