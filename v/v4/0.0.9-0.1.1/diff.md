# Comparing `tmp/v4-0.0.9.tar.gz` & `tmp/v4-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/v4-0.0.9.tar", last modified: Wed Jun 22 15:54:35 2022, max compression
+gzip compressed data, was "v4-0.1.1.tar", last modified: Thu Jul 27 01:07:12 2023, max compression
```

## Comparing `v4-0.0.9.tar` & `v4-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2022-06-22 15:54:35.310652 v4-0.0.9/
--rw-r--r--   0 root         (0) staff       (20)      302 2022-06-22 15:54:35.310429 v4-0.0.9/PKG-INFO
--rwxrwxrwx   0 root         (0) staff       (20)      838 2018-04-12 20:31:22.000000 v4-0.0.9/README.md
--rw-r--r--   0 root         (0) staff       (20)       38 2022-06-22 15:54:35.310713 v4-0.0.9/setup.cfg
--rwxrwxrwx   0 root         (0) staff       (20)      385 2022-06-22 15:49:45.000000 v4-0.0.9/setup.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2022-06-22 15:54:35.308960 v4-0.0.9/v4/
--rwxrwxrwx   0 root         (0) staff       (20)        2 2017-12-29 23:35:19.000000 v4-0.0.9/v4/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     7515 2022-06-22 15:52:39.000000 v4-0.0.9/v4/vd.py
--rwxr-xr-x   0 root         (0) staff       (20)    24619 2022-06-22 15:52:27.000000 v4-0.0.9/v4/vx.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2022-06-22 15:54:35.310185 v4-0.0.9/v4.egg-info/
--rwxrwxrwx   0 root         (0) staff       (20)      302 2022-06-22 15:54:35.000000 v4-0.0.9/v4.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) staff       (20)      155 2022-06-22 15:54:35.000000 v4-0.0.9/v4.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) staff       (20)        1 2022-06-22 15:54:35.000000 v4-0.0.9/v4.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) staff       (20)        3 2022-06-22 15:54:35.000000 v4-0.0.9/v4.egg-info/top_level.txt
+drwxr-xr-x   0 reeves     (501) staff       (20)        0 2023-07-27 01:07:12.628681 v4-0.1.1/
+-rwxrwxrwx   0 reeves     (501) staff       (20)    35148 2014-09-08 17:52:36.000000 v4-0.1.1/LICENSE.txt
+-rw-r--r--   0 reeves     (501) staff       (20)      288 2023-07-27 01:07:12.628508 v4-0.1.1/PKG-INFO
+-rwxrwxrwx   0 reeves     (501) staff       (20)      838 2018-04-12 20:31:22.000000 v4-0.1.1/README.md
+-rw-r--r--   0 reeves     (501) staff       (20)       38 2023-07-27 01:07:12.628731 v4-0.1.1/setup.cfg
+-rwxrwxrwx   0 reeves     (501) staff       (20)      384 2023-07-27 01:05:40.000000 v4-0.1.1/setup.py
+drwxr-xr-x   0 reeves     (501) staff       (20)        0 2023-07-27 01:07:12.627583 v4-0.1.1/v4/
+-rwxrwxrwx   0 reeves     (501) staff       (20)        2 2017-12-29 23:35:19.000000 v4-0.1.1/v4/__init__.py
+-rw-r--r--   0 reeves     (501) staff       (20)    12327 2023-07-27 00:50:11.000000 v4-0.1.1/v4/vd.py
+-rwxr-xr-x   0 reeves     (501) staff       (20)    28090 2023-07-27 00:50:03.000000 v4-0.1.1/v4/vx.py
+drwxr-xr-x   0 reeves     (501) staff       (20)        0 2023-07-27 01:07:12.628311 v4-0.1.1/v4.egg-info/
+-rwxrwxrwx   0 reeves     (501) staff       (20)      288 2023-07-27 01:07:12.000000 v4-0.1.1/v4.egg-info/PKG-INFO
+-rwxrwxrwx   0 reeves     (501) staff       (20)      167 2023-07-27 01:07:12.000000 v4-0.1.1/v4.egg-info/SOURCES.txt
+-rwxrwxrwx   0 reeves     (501) staff       (20)        1 2023-07-27 01:07:12.000000 v4-0.1.1/v4.egg-info/dependency_links.txt
+-rwxrwxrwx   0 reeves     (501) staff       (20)        3 2023-07-27 01:07:12.000000 v4-0.1.1/v4.egg-info/top_level.txt
```

### Comparing `v4-0.0.9/README.md` & `v4-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `v4-0.0.9/v4/vx.py` & `v4-0.1.1/v4/vx.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,38 +30,45 @@
     out=subprocess.check_output( cmd, shell=True).decode()
     #p = subprocess.Popen(cmd, stdout=subprocess.PIPE, shell=True)
     #out, _ = p.communicate()
     #### python does not like a variable name "if" change to "vxif"
     olist = re.sub("if=", "vxif=", out )
     return olist
 
-def vaparse(*args):
+from copy import deepcopy
+def vaparse(argst,**kwargs):
     '''parse command line arguments using v4 rules
     returns a dict with matched arguments
-    any unmathed args are returned in a list celled umatch
+    any unmatched args are returned in a list celled umatch
     '''
     rdict = {}
     slist = {}
     mlist = []
     alist = []
     umatch = []
-    if len(args) == 2:
-        ilist = args[1]
+    if 'args' in kwargs:
+        xilist = kwargs['args']
     else:
-        ilist = sys.argv
-    qlist = args[0].split()
+        xilist = sys.argv
+    ilist=deepcopy(xilist)
+    qlist = argst.split()
+    if 'pname' not in kwargs:
+        del ilist[0]
     for i in qlist:
         if i[0] == '-':
             mlist.append(i)
         else:
             alist.append(i)
     for i in ilist:
-        if i in mlist:
+        if 0 == i.find('-'):
+          if i in mlist:
             rdict[i] = i
             mlist.remove(i)
+          else:
+            umatch.append(i)
         else:
             index = i.find('=')
             if index != -1:
                 key = i[:index+1]
                 if key in alist:
                     rdict[key[:len(key)-1]] = i[index+1:]
                     alist.remove(key)
@@ -94,15 +101,15 @@
 vnptypes = (np.byte, np.ubyte, np.short, np.single, np.double, np.byte, np.ubyte, np.intc, "x", "x")
 
 if __name__ == '__main__':
      import sys
     #sys.exit(main(sys.argv))
 
 #vxfreadelem
-#reads an elemdn from a file 
+#reads an element from a file 
 # returns key and data 
 
 def vxfreadelem ( f ):
         """ read a vx element from an opened file"""
         global elcodes, vxdtypes, vxdlens
         elemr = f.read (4 )
         if ( len(elemr) != 4 ):
@@ -113,14 +120,15 @@
         if ( len(eleml) != 4 ):
             return (("EOF", 0, ""))
         elen = struct.unpack('i', eleml) [0] 
         #print (hex(elem))
         #print (hex(elem))
         key = hex(elem)
         base= elem & 0xf
+        #print (elem)
         if key in elcodes:
             elname = elcodes[key] 
             #print ("%s: %s (%s)" % (key, elname, elen ))
         else:
             return (("EOF", 0, ""))
         if  base == 10 :
              return ((elname, elen, ""))
@@ -131,15 +139,17 @@
                  return (("EOF", 0, ""))
         #print ( "base is %i " % base)
         if base == 0:
                  data = edata.decode('UTF-8')
                  return ((elname, data, ""))
         else:
                  #print (" edata length %i" % len(edata))
-                 data = struct.unpack( "%d%s" % (elen//vxdlens[base], vxdtypes[base]) , edata)
+                 # the "<" was added to enforce little-endian needed for long int?
+                 # thus will likely not work on big-endian?
+                 data = struct.unpack( "<%d%s" % (elen//vxdlens[base], vxdtypes[base]) , edata)
                  return ((elname, data, vnptypes[base]))
 
 
 #vxfopen opens file and reads vx header
 def vxfopen ( fname ):
     """ open a vx file """
     cmd = ""
@@ -155,15 +165,18 @@
       #print (key)
       if key == "EOF":
            return (vf, key) 
       if key == "VX_FCMND":
            cmd = data 
     #print (data)
       if key == "VX_FHIST":
-           return (vf, data + cmd)
+           if data[-1] != '\n' and data[-2] != '\n' :
+               return (vf, data + '\n' + cmd)
+           else:
+               return (vf, data + cmd)
     return (vf, "EOF")
 
 # read a single image
 def vxfrdim(fd, vxst):
     frame = False
     pchan = 1
     while True:
@@ -237,14 +250,16 @@
              rnptype = nptype
              status = True
              if not frame:
                   break
     return (status, xs, ys, pchan, rnptype, idata )
 
 # read all images 2D and 3D
+# need to fix not status on first image (error) 11/4/22
+# need to add error return
 def vxfrdaim(fd, vxst):
     imt = ()
     ishape = ()
     cnt = 0
     while True:
         status, ixs, iys, ichan, inptype, imdata = vxffrdim(fd)
         #print ("resp" , status, ixs, iys, inptype, len(imdata))
@@ -304,15 +319,15 @@
         if ( 3 == vxst.i.ndim ):
             vxst.c = 3;
         vxst.h = "VisionX V4 import %s" % name
       else:
         vxst = vxfread(name)
     else:
         if type(name)  == np.ndarray:
-             vxst.i = name
+             vxst.i = np.copy(name)
              #check if 2 or 3 channels possible (a guess)
 
              if name.ndim > 2:
                 chan = name.shape[ name.ndim-1]
                 if chan > 1 and chan < 4:
                     vxst.c = chan
         else:
@@ -328,19 +343,20 @@
 
 
 
 def vxfwopen ( fname, cmnd, hist ):
     """ open file and write a vx header"""
     cmnd += '\n'
     xf = open(fname, "wb")
+    xfname = fname + ' '
     mach = 'Lendian\n'
     xf.write(b'#vIsX\n')
     xf.write (struct.pack('I', eldcodes['VX_FNAME']))
-    xf.write (struct.pack('I',len(fname)))
-    xf.write (bytearray(fname.encode()))
+    xf.write (struct.pack('I',len(xfname )))
+    xf.write (bytearray(xfname.encode()))
     xf.write (struct.pack('I', eldcodes['VX_FCMND']))
     xf.write (struct.pack('I',len(cmnd)))
     xf.write (bytearray(cmnd.encode()))
     xf.write (struct.pack('I', eldcodes['VX_FMACH']))
     xf.write (struct.pack('I',len(mach)))
     xf.write (bytearray(mach.encode()))
     xf.write (struct.pack('I', eldcodes['VX_FUID']))
@@ -361,26 +377,26 @@
     xf.write (struct.pack('I', eldcodes['VX_FRAME']))
     xf.write (struct.pack('I',idx))
     xf.write (struct.pack('I', eldcodes['VX_BBX']))
     xf.write (struct.pack('I',24))
     xf.write (bbx)
     ### figure nel and fmt
     tag = 'VX_PBYTE'
-    if type == np.byte:
+    if etype == np.byte:
         tag = 'VX_PCHAR'
-    elif type == np.short:
+    elif etype == np.short:
         tag = 'VX_PSHORT'
         nel *= 2
-    elif type == np.intc:
+    elif etype == np.intc:
         tag = 'VX_PINT'
         nel *= 4
-    elif type == np.single:
+    elif etype == np.single:
         tag = 'VX_PFLOAT'
         nel *= 4
-    elif type == np.double:
+    elif etype == np.double:
         tag = 'VX_PDOUBLE'
         nel *= 8
     xf.write (struct.pack('I', eldcodes[tag]))
     xf.write (struct.pack('I',nel))
     xf.write (im)
     xf.write (struct.pack('I', eldcodes['VX_EFRAME']))
     xf.write (struct.pack('I',idx))
@@ -392,32 +408,39 @@
     if fileext in ('.png', '.gif', '.tif','.tiff','pdf','jpg','jpeg'):
         if not threed:
             Image.fromarray(vxst.i).save(fname)
         else:
             Image.fromarray(vxst.i[0]).save(fname)
         return
     idx = 1
-    xf = vxfwopen(fname, "vx.py write", 'no-history\n')
+    hist = vxst.h
+    cmnd = vxst.cmd
+    if len(hist) == 0:
+        hist='no-history '
+    if len(cmnd) == 0:
+        cmnd='vx.py write'
+    # traditionally cmnd and hist end in 0 
+    xf = vxfwopen(fname, cmnd, hist)
     bbx = np.zeros(6, dtype=np.single)
     bbx[5]= 1.0
     if not threed:
         bbx[1] = vxst.i.shape[1]
         bbx[3] = vxst.i.shape[0]
         vximwrite(xf, vxst.i, bbx, idx, vxst.c)
     else:
         n = vxst.i.shape[0]
         idx = 0
         while idx < n:
             im = vxst.i[idx]
-            bbx[1] = vxst.i.shape[1] // vxst.c
-            bbx[3] = vxst.i.shape[0]
+            bbx[1] = im.shape[1]
+            bbx[3] = im.shape[0]
             bbx[4] = idx
             idx += 1
             bbx[5] = idx
-            vximwrite(xf, im, bbx, idx)
+            vximwrite(xf, im, bbx, idx, vxst.c)
     xf.close()
 #-------------------------------------#
 
 def vfread ( file ):
    tname = file + ".npy"
    os.system("vxtonpy if=" + file + " of=" + tname)
    a = load( tname )
@@ -473,16 +496,32 @@
 def v3fnewim ( type, bbx, chan ):
     if type == 1 or type == "VX_PCHAN":
         type = 'uint8'
     stm = (bbx[5] , bbx[3], bbx[1] * chan)
     tm = np.zeros( stm, dtype=type)
     return tm
 
+def is_notebook() -> bool:
+    try:
+        shell = get_ipython().__class__.__name__
+        if shell == 'ZMQInteractiveShell':
+            return True   # Jupyter notebook or qtconsole
+        elif shell == 'TerminalInteractiveShell':
+            return False  # Terminal running IPython
+        else:
+            return False  # Other type (?)
+    except NameError:
+        return False      # Probably standard Python interpreter
+
 class Vx:
    def __init__(self, *args):
+     if is_notebook():
+        self.cmd = 'interactive'
+     else:
+        self.cmd = ' '.join(sys.argv)
      if 0 == len(args) :
         self.i = np.zeros([0,0],'uint8')
         self.h = ''
         self.c = 1
         return
      if 1 == len(args) :
        # read image file
@@ -580,15 +619,60 @@
                  stm = (zlo +zhi + self.i.shape[0], ylo + yhi + self.i.shape[1],
                        xlo + xhi + self.i.shape[2])
                  self.i = np.zeros( stm, dtype=vxin.dtype )
                  for z in range(vxin.shape[0]):
                      for y in range(vxin.shape[1]):
                        for x in range(vxin.shape[2]):
                          self.i[z+zlo,y+ylo,x+xlo] = vxin[z,y,x]
+#----------------
+# list based vx file io
+def vrfile ( fname ):
+    body  = []
+    head = ""
+    (fd, head) = vxfopen (fname )
+    ## check on correct open
+    if  0 == len(head):
+        fd.close()
+        return (head, body)
 
+    while True:
+        (key, data, nptype) = vxfreadelem(fd)
+        if key == 'EOF':
+                   break
+        base = eldcodes[key] & 0xf 
+        if base == 10 or base == 0 :
+          body.append((key, data))
+        else:
+          body.append((key, np.asarray(data, dtype=nptype)))
+    fd.close()
+    return ( head, body )
+
+def vwfile ( fname, head, body, cmnd="vx.py-write" ):
+    fd = vxfwopen(fname, cmnd, head)
+    for (tag, val) in body:
+      # write tag
+      fd.write (struct.pack('I', eldcodes[tag]))
+      # find data length for val
+      # for type 0
+      base = eldcodes[tag] & 0xf 
+      if base == 10 :
+          fd.write (struct.pack('I',val))
+      elif base == 0 :
+          fd.write (struct.pack('I',len(val)))
+          fd.write (bytearray(val.encode()))
+          # other types
+          # need to ensure val is correct type for tag
+          # and deep copy if necessary
+      else:
+         nel = len(val) * vxdlens[base]
+         fd.write (struct.pack('I',nel))
+         fd.write (np.asarray(val, dtype=vnptypes[base]))
+    fd.close()
+
+#----------------
 __VXtmp = [];
 __VXtmc = 1;
 __VXresp ='foo'
 __VXrim =''
 
 def vxxread(rfile ):
         vxx = Vx();
@@ -719,7 +803,35 @@
                 dolist += ' ' + j[0] + '\' + vx.vdovar("__VXtmp") + \''
             else:
                 dolist += ' ' + j[0] + '\' + vx.vdovar(' + j[1] + ') + \''
         else:
             dolist += ' ' + i
             #print i
     return plist + dolist + polist;
+def vxinfo( vxarg):
+    #if type(vxim)  == np.ndarray:
+    res = {}
+    vxim = vx.vximp(vxarg)
+    res['shape'] = np.shape(vxim.i)
+    res['dtype'] = vxim.i.dtype
+    #res[bbox'] = vxim.bbx
+    res['color'] = vxim.c == 3
+    return res
+
+def vxstats( vxarg):
+    res = {}
+    vxim = vx.vximp(vxarg)
+    res['mean'] = round(np.mean(vxim.i), 5)
+    res['median'] = round(np.median(vxim.i), 5)
+    res['min'] = round(np.min(vxim.i), 5)
+    res['max'] = round(np.max(vxim.i), 5)
+    res['std'] = round(np.std(vxim.i), 5)
+    vq = vxim.i.astype(float)
+    #vq = np.where(vxim.i == 0, 'NaN',vq)
+    vq[vxim.i==0] = np.nan
+    res['mean0'] = round(np.nanmean(vq), 5)
+    res['median0'] = round(np.nanmedian(vq), 5)
+    res['min0'] = round(np.nanmin(vq), 5)
+    res['max0'] = round(np.nanmax(vq), 5)
+    res['std0'] = round(np.nanstd(vq), 5)
+    return res
+
```

