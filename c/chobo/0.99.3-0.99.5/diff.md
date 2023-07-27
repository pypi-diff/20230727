# Comparing `tmp/chobo-0.99.3.tar.gz` & `tmp/chobo-0.99.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\chobo-0.99.3.tar", last modified: Sun Oct 18 02:19:09 2020, max compression
+gzip compressed data, was "chobo-0.99.5.tar", last modified: Thu Jul 27 18:18:25 2023, max compression
```

## Comparing `chobo-0.99.3.tar` & `chobo-0.99.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2020-10-18 02:19:09.595108 chobo-0.99.3/
--rw-rw-rw-   0        0        0     1477 2020-10-18 02:19:09.595108 chobo-0.99.3/PKG-INFO
--rw-rw-rw-   0        0        0      850 2020-10-18 02:13:03.000000 chobo-0.99.3/README.md
-drwxrwxrwx   0        0        0        0 2020-10-18 02:19:05.682144 chobo-0.99.3/chobo/
--rw-rw-rw-   0        0        0    36621 2020-10-18 02:08:43.000000 chobo-0.99.3/chobo/__init__.py
-drwxrwxrwx   0        0        0        0 2020-10-18 02:19:09.594149 chobo-0.99.3/chobo.egg-info/
--rw-rw-rw-   0        0        0     1477 2020-10-18 02:19:09.000000 chobo-0.99.3/chobo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      180 2020-10-18 02:19:09.000000 chobo-0.99.3/chobo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-10-18 02:19:09.000000 chobo-0.99.3/chobo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2020-10-18 02:19:09.000000 chobo-0.99.3/chobo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2020-10-18 02:19:09.000000 chobo-0.99.3/chobo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2020-10-18 02:19:09.596069 chobo-0.99.3/setup.cfg
--rw-rw-rw-   0        0        0      821 2020-10-18 02:09:06.000000 chobo-0.99.3/setup.py
+drwxr-xr-x   0 clee       (501) staff       (20)        0 2023-07-27 18:18:25.100509 chobo-0.99.5/
+-rw-r--r--   0 clee       (501) staff       (20)    35149 2023-07-24 12:09:08.000000 chobo-0.99.5/LICENSE
+-rw-r--r--   0 clee       (501) staff       (20)     1365 2023-07-27 18:18:25.100403 chobo-0.99.5/PKG-INFO
+-rw-r--r--   0 clee       (501) staff       (20)      834 2023-07-24 12:09:08.000000 chobo-0.99.5/README.md
+drwxr-xr-x   0 clee       (501) staff       (20)        0 2023-07-27 18:18:25.099373 chobo-0.99.5/chobo/
+-rw-r--r--   0 clee       (501) staff       (20)    38591 2023-07-24 17:08:46.000000 chobo-0.99.5/chobo/__init__.py
+drwxr-xr-x   0 clee       (501) staff       (20)        0 2023-07-27 18:18:25.100264 chobo-0.99.5/chobo.egg-info/
+-rw-r--r--   0 clee       (501) staff       (20)     1365 2023-07-27 18:18:25.000000 chobo-0.99.5/chobo.egg-info/PKG-INFO
+-rw-r--r--   0 clee       (501) staff       (20)      166 2023-07-27 18:18:25.000000 chobo-0.99.5/chobo.egg-info/SOURCES.txt
+-rw-r--r--   0 clee       (501) staff       (20)        1 2023-07-27 18:18:25.000000 chobo-0.99.5/chobo.egg-info/dependency_links.txt
+-rw-r--r--   0 clee       (501) staff       (20)        6 2023-07-27 18:18:25.000000 chobo-0.99.5/chobo.egg-info/top_level.txt
+-rw-r--r--   0 clee       (501) staff       (20)      751 2023-07-24 17:41:47.000000 chobo-0.99.5/pyproject.toml
+-rw-r--r--   0 clee       (501) staff       (20)       38 2023-07-27 18:18:25.100537 chobo-0.99.5/setup.cfg
```

### Comparing `chobo-0.99.3/README.md` & `chobo-0.99.5/README.md`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-# chobo
-
-The chobo module is a forked version of the [intrographics](http://myslu.stlawu.edu/~ltorrey/intrographics/) module developed by [Dr. Lisa Torrey](http://myslu.stlawu.edu/~ltorrey/).
-
-It allows you to create graphical displays in your Python 3 programs.
-The name chobo (초보) is a Korean word that means a beginner/novice, and the name is to inspire beginners at programming to give it a try.
-
-It is written in [Python 3](https://www.python.org/), and uses the [pygame](https://www.pygame.org/) module as the back-end, and adds the following features:
-
-* Image files other than just GIF
-* Arc as a new shape
-* An empty image shape
-* Shape rotations
-* Use of any system fonts
-* Sound/music files and their playback
-
+# chobo
+
+The chobo module is a forked version of the [intrographics](http://myslu.stlawu.edu/~ltorrey/intrographics/) module developed by [Dr. Lisa Torrey](http://myslu.stlawu.edu/~ltorrey/).
+
+It allows you to create graphical displays in your Python 3 programs.
+The name chobo (초보) is a Korean word that means a beginner/novice, and the name is to inspire beginners at programming to give it a try.
+
+It is written in [Python 3](https://www.python.org/), and uses the [pygame](https://www.pygame.org/) module as the back-end, and adds the following features:
+
+* Image files other than just GIF
+* Arc as a new shape
+* An empty image shape
+* Shape rotations
+* Use of any system fonts
+* Sound/music files and their playback
+
 The full documentation is available in the [doc](https://github.com/choongsoo/chobo/tree/master/doc) folder.
```

### Comparing `chobo-0.99.3/chobo/__init__.py` & `chobo-0.99.5/chobo/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,20 +85,23 @@
         self.fps = 200
         self.tick = 0
 
         self.shapes = []
 
         self.timerFunctions = {}
 
-        self.keyFunctions = []
+        self.pressedKeys = set()
+        self.typedKeyFunctions = set()
+        self.pressedKeyFunctions = set()
 
         self.mouseClickFunctions = {}
         self.mouseDragFunctions = {}
         self.mouseDown = {}
 
+
         sys.window = self
 
     def onTimer(self, interval=None, timerFunc=None, *extra):
         """Add a function on a timer"""
         command = "window.onTimer(interval,function)"
 
         # Argument existence
@@ -147,18 +150,18 @@
             system.invalid("buttonID", buttonID)
             return
         if buttonID < 1 or buttonID > 5:
             system.invalid("buttonID", buttonID)
             return
 
         if buttonID not in self.mouseClickFunctions:
-            self.mouseClickFunctions[buttonID] = []
+            self.mouseClickFunctions[buttonID] = set()
 
         if clickFunc not in self.mouseClickFunctions[buttonID]:
-            self.mouseClickFunctions[buttonID].append(clickFunc)
+            self.mouseClickFunctions[buttonID].add(clickFunc)
 
     def offMouseClick(self, buttonID, clickFunc, *extra):
         """Unassign a function to handle mouse button clicks."""
         command = "window.offMouseClick(buttonID, function)"
 
         # Argument existence
         if len(extra) > 0:
@@ -171,15 +174,15 @@
         except:
             system.invalid("buttonID", buttonID)
             return
         if buttonID < 1 or buttonID > 5:
             system.invalid("buttonID", buttonID)
             return
 
-        if clickFunc in self.mouseClickFunctions.get(buttonID, []):
+        if clickFunc in self.mouseClickFunctions.get(buttonID, set()):
             self.mouseClickFunctions[buttonID].remove(clickFunc)
 
     def onMouseDrag(self, buttonID, dragFunc, *extra):
         """Assign a function to handle mouse drags."""
         command = "window.onMouseDrag(buttonID, function)"
 
         # Argument existence
@@ -194,18 +197,18 @@
             system.invalid("buttonID", buttonID)
             return
         if buttonID < 1 or buttonID > 5:
             system.invalid("buttonID", buttonID)
             return
 
         if buttonID not in self.mouseDragFunctions:
-            self.mouseDragFunctions[buttonID] = []
+            self.mouseDragFunctions[buttonID] = set()
 
         if dragFunc not in self.mouseDragFunctions[buttonID]:
-            self.mouseDragFunctions[buttonID].append(dragFunc)
+            self.mouseDragFunctions[buttonID].add(dragFunc)
 
     def offMouseDrag(self, buttonID, dragFunc, *extra):
         """Unassign a function to handle mouse drags."""
         command = "window.offMouseDrag(buttonID, function)"
 
         # Argument existence
         if len(extra) > 0:
@@ -218,15 +221,15 @@
         except:
             system.invalid("buttonID", buttonID)
             return
         if buttonID < 1 or buttonID > 5:
             system.invalid("buttonID", buttonID)
             return
 
-        if dragFunc in self.mouseDragFunctions.get(buttonID, []):
+        if dragFunc in self.mouseDragFunctions.get(buttonID, set()):
             self.mouseDragFunctions[buttonID].remove(dragFunc)
 
     def translateKey(self, key):
         return pygame.key.name(key)
 
     def open(self, title="chobo", *extra):
         """Make the window visible."""
@@ -244,19 +247,22 @@
 
         while running:
             for event in pygame.event.get():
                 if event.type == pygame.QUIT:
                     running = False
                 elif event.type == pygame.KEYDOWN and pygame.key.get_focused():
                     pressedKey = self.translateKey(event.key)
+                    self.pressedKeys.add(pressedKey)
                     if DEBUG:
                         print(pressedKey)
-                    if len(self.keyFunctions) > 0:
-                        for aFunction in self.keyFunctions:
-                            aFunction(pressedKey)
+                elif event.type == pygame.KEYUP and pygame.key.get_focused():
+                    pressedKey = self.translateKey(event.key)
+                    self.pressedKeys.remove(pressedKey)
+                    for aFunction in self.typedKeyFunctions:
+                        aFunction(pressedKey)
                 elif pygame.mouse.get_focused():
                     if event.type == pygame.MOUSEBUTTONDOWN:
                         self.mouseDown[event.button] = True
                         clickFunctions = self.mouseClickFunctions.get(event.button, [])
                         x, y = event.pos
                         if DEBUG:
                             print(event.button, (x, y))
@@ -268,66 +274,92 @@
                         for mouseButton in dict(self.mouseDragFunctions):
                             if self.mouseDown.get(mouseButton, False):
                                 dragFunctions = self.mouseDragFunctions.get(mouseButton, [])
                                 x, y = event.pos
                                 for aFunction in dragFunctions[:]:
                                     aFunction(x, y)
 
-            # refresh drawing
+            for pressedKey in self.pressedKeys:
+                for aFunction in self.pressedKeyFunctions:
+                    aFunction(pressedKey)
 
             # set the background color
             self.screen.fill(self.background)
 
             # draw all the shapes
             for aShape in self.shapes:
                 aShape.__draw__()
 
-
             # force an update
             pygame.display.flip()
 
-            #iwait for the interval
+            # wait for the interval
             self.tick += self.clock.tick(self.fps)
 
             # call all the timer functions
             for interval in dict(self.timerFunctions):
                 if self.tick - self.timerFunctions[interval]["lastRun"] > interval:
                     self.timerFunctions[interval]["lastRun"] = self.tick
                     for aFunction in self.timerFunctions[interval]["functions"][:]:
                         aFunction()
-
         pygame.quit()
 
+    def onKeyType(self, keyFunc=None, *extra):
+        """Assign a function to handle key types."""
+        command = "window.onKeyType(function)"
+
+        # Argument existence
+        if len(extra) > 0:
+            return system.extra(command)
+        if keyFunc is None:
+            system.missing(command)
+            return
+
+        self.typedKeyFunctions.add(keyFunc)
+
+    def offKeyType(self, keyFunc=None, *extra):
+        """Unassign a function to handle key types."""
+        command = "window.offKeyType(function)"
+
+        # Argument existence
+        if len(extra) > 0:
+            return system.extra(command)
+        if keyFunc is None:
+            system.missing(command)
+            return
+
+        if keyFunc in self.typedKeyFunctions:
+            self.typedKeyFunctions.remove(keyFunc)
+
     def onKeyPress(self, keyFunc=None, *extra):
         """Assign a function to handle key presses."""
-        command = "window.onKeyPress(function)"
+        command = "window.onKeyType(function)"
 
         # Argument existence
         if len(extra) > 0:
             return system.extra(command)
         if keyFunc is None:
             system.missing(command)
             return
 
-        if keyFunc not in self.keyFunctions:
-            self.keyFunctions.append(keyFunc)
+        self.pressedKeyFunctions.add(keyFunc)
 
     def offKeyPress(self, keyFunc=None, *extra):
-        """Unassign a function to handle mouse drags."""
-        command = "window.offKeyPress(function)"
+        """Unassign a function to handle key presses."""
+        command = "window.offKeyType(function)"
 
         # Argument existence
         if len(extra) > 0:
             return system.extra(command)
         if keyFunc is None:
             system.missing(command)
             return
 
-        if keyFunc in self.keyFunctions:
-            self.keyFunctions.remove(keyFunc)
+        if keyFunc in self.pressedKeyFunctions:
+            self.pressedKeyFunctions.remove(keyFunc)
 
     def fill(self, color=None, *extra):
         """Give the window a background color."""
         command = "window.fill(color)"
 
         # Argument existence
         if len(extra) > 0:
@@ -641,15 +673,15 @@
             angle = float(angle)
         except ValueError:
             return system.invalid("invalid angle", angle)
 
         # convert from degrees to radians
         angle = math.radians(angle)
 
-        return (x + width * math.sin(angle) + width, y - height * math.cos(angle) + height)
+        return (x + width * math.sin(angle), y - height * math.cos(angle))
 
 class windowshape:
     def __init__(self):
         self.rect = None
 
     def getRect(self):
         return self.rect
@@ -679,40 +711,38 @@
     def __init__(self, points):
         super().__init__()
         self.configure(points)
 
     # Update the shape location.
     def configure(self, points):
         self.points = points
-        self.x = min(x for (x,y) in points)
-        self.y = min(y for (x,y) in points)
         self.__dict__["left"] = min(x for (x,y) in points)
         self.__dict__["top"] = min(y for (x,y) in points)
         self.__dict__["right"] = max(x for (x,y) in points)
         self.__dict__["bottom"] = max(y for (x,y) in points)
         self.__dict__["width"] = self.__dict__["right"] - self.__dict__["left"]
         self.__dict__["height"] = self.__dict__["bottom"] - self.__dict__["top"]
-        self.rect = pygame.Rect(self.x, self.y, self.__dict__["width"], self.__dict__["height"])
+        self.rect = pygame.Rect(self.__dict__["left"], self.__dict__["top"], self.__dict__["width"], self.__dict__["height"])
+
+        self.x = (self.__dict__["left"] + self.__dict__["right"]) // 2
+        self.y = (self.__dict__["top"] + self.__dict__["bottom"]) // 2
 
     def rotate(self, angle):
         angle = math.radians(angle)
 
-        cx = self.__dict__["left"] + self.__dict__["width"] / 2
-        cy = self.__dict__["top"] + self.__dict__["height"] / 2
-
         newPoints = []
         for index in range(len(self.points)):
             x, y = self.points[index]
-            dx = x - cx
-            dy = y - cy
+            dx = x - self.x
+            dy = y - self.y
             newx = dx * math.cos(angle) - dy * math.sin(angle)
             newy = dy * math.cos(angle) + dx * math.sin(angle)
 
-            newx += cx
-            newy += cy
+            newx += self.x
+            newy += self.y
             newPoints.append((newx, newy))
         self.configure(newPoints)
 
     def fill(self, color=None, *extra):
         """Change the color of this shape."""
         command = self.__class__.__name__ + ".fill(color)"
 
@@ -752,42 +782,43 @@
             return system.extra(command)
         if pos is None:
             return system.missing(command)
 
         # Argument types
         try:
             x, y = pos
-            sx, sy = self.__dict__["left"], self.__dict__["top"]
-            dx = int(x) - sx
-            dy = int(y) - sy
+            dx = int(x) - self.x
+            dy = int(y) - self.y
         except ValueError:
             return system.invalid("new location", pos)
 
         self.move(dx, dy)
 
-    def scale(self, horizonScale=None, verticalScale=None, *extra):
+    def scale(self, horizontalScale=None, verticalScale=None, *extra):
         """Scale this shape by the given horizontal and vertical scale."""
         command = self.__class__.__name__ + ".scale(horizonScale,verticalScale)"
 
         # Argument existence
         if len(extra) > 0:
             return system.extra(command)
-        if horizonScale is None or verticalScale is None:
+        if horizontalScale is None or verticalScale is None:
             return system.missing(command)
+        if horizontalScale <= 0 or verticalScale <= 0:
+            return system.invalid("scales ", (horizontalScale, verticalScale))
 
         newPoints = []
         for index in range(len(self.points)):
             x, y = self.points[index]
-            dx = x - self.__dict__["left"]
-            dy = y - self.__dict__["top"]
-            newx = dx * horizonScale
+            dx = x - self.x
+            dy = y - self.y
+            newx = dx * horizontalScale
             newy = dy * verticalScale
 
-            newx += self.__dict__["left"]
-            newy += self.__dict__["top"]
+            newx += x
+            newy += y
             newPoints.append((newx, newy))
         self.configure(newPoints)
 
 class lines(listshape):
     """A line shape."""
     def __init__(self, points):
         super().__init__(points)
@@ -877,39 +908,36 @@
             pygame.draw.polygon(sys.window.screen, self.__dict__["fillColor"], self.points, 0)
 
         super().__draw__(enclosed=True)
 
 class rectangle(polygon):
     """A polygon shape."""
     def __init__(self, x, y, width, height):
-        points = [(x, y), (x + width, y), (x + width, y + height), (x, y + height)]
+        points = [(x - width / 2, y - height / 2), (x + width / 2, y - height / 2), (x + width / 2, y + height / 2),  (x - width / 2, y + height / 2)]
         super().__init__(points)
 
 class arc(polygon):
     """An arc shape."""
 
     def __init__(self, x, y, width, height, beginAngle, arcAngle):
-#        self.id = canvas.create_oval(0, 0, 0, 0, width=1)
         points = []
 
         a = max(1, int(width / 2))
         b = max(1, int(height / 2))
 
         arcAngle %= 360
 
         if arcAngle == 0:
             arcAngle = 360
         else:
-            points.append((x + a, y + b))
+            points.append((x, y))
 
         for i in range(beginAngle, beginAngle + arcAngle + 1):
             points.append(sys.window.ovalPoint( (x, y), width, height, i))
 
-        # points = [(v + x + a, w + y + b) for (v, w) in points]
-
         super().__init__(points)
 
 class oval(arc):
     """An oval shape."""
     def __init__(self, x, y, width, height):
         super().__init__(x, y, width, height, 0, 360)
 
@@ -972,38 +1000,58 @@
 class image(pointshape):
     """A image."""
 
     def __init__(self, x, y, filename=None):
         if filename is not None:
             self.img = pygame.image.load(filename)
             self.original = pygame.image.load(filename)
+            self.scaledImage = pygame.image.load(filename)
         super().__init__(x, y)
         self.rotation = 0
 
     # Update the shape location.
     def configure(self, x, y):
         self.x = x
         self.y = y
-        self.__dict__["left"] = x
-        self.__dict__["top"] = y
         self.__dict__["width"] = self.img.get_width()
         self.__dict__["height"] = self.img.get_height()
-        self.__dict__["right"] = x + self.img.get_width()
-        self.__dict__["bottom"] = y + self.img.get_height()
+        self.__dict__["left"] = self.x - self.__dict__["width"] // 2
+        self.__dict__["top"] = self.y - self.__dict__["height"] // 2
+        self.__dict__["right"] = self.x + self.__dict__["width"] // 2
+        self.__dict__["bottom"] = self.y + self.__dict__["height"] // 2
         self.__dict__["rect"] = self.getRect()
 
     def rotate(self, angle):
         if angle == 0:
             return
         self.rotation += angle
+
         del self.img
-        self.img = pygame.transform.rotate(self.original, -self.rotation)
-        x = self.x + self.__dict__["width"] / 2 - self.img.get_width() / 2
-        y = self.y + self.__dict__["height"] / 2 - self.img.get_height() / 2
-        self.configure(x, y)
+        self.img = pygame.transform.rotate(self.scaledImage, -self.rotation)
+
+        self.configure(self.x, self.y)
+
+    def scale(self, horizontalScale=None, verticalScale=None, *extra):
+        command = self.__class__.__name__ + ".scale(horizonScale,verticalScale)"
+
+        # Argument existence
+        if len(extra) > 0:
+            return system.extra(command)
+        if horizontalScale is None or verticalScale is None:
+            return system.missing(command)
+        if horizontalScale <= 0 or verticalScale <= 0:
+            return system.invalid("scales ", (horizontalScale, verticalScale))
+
+        del self.scaledImage
+        self.scaledImage = pygame.transform.scale(self.original, (horizontalScale * self.original.get_width(), verticalScale * self.original.get_height()))
+        if self.rotation != 0:
+            del self.img
+            self.img = pygame.transform.rotate(self.scaledImage, -self.rotation)
+
+        self.configure(self.x, self.y)
 
     def getColor(self, pos=None, *extra):
         """Retrieve the (r,g,b) color at pixel x,y of the image."""
         command = "image.getColor( (x,y) )"
 
         # Argument existence
         if len(extra) > 0:
@@ -1049,30 +1097,29 @@
         try:
             r, g, b = color
         except:
             return system.invalid("color", color)
         self.original.set_at( (x, y), (r, g, b, 255))
 
         self.img = self.original
-        self.rotate(self.rotation)
 
     def saveAs(self, filename=None, *extra):
         """Save this image to a file."""
         command = "image.saveAs(filename)"
 
         # Argument existence
         if len(extra) > 0:
             return system.extra(command)
         if filename is None:
             return system.missing(command)
 
         pygame.image.save(self.img, str(filename))
 
     def getRect(self):
-        return pygame.Rect(self.x, self.y, self.img.get_width(), self.img.get_height())
+        return pygame.Rect(self.x - self.img.get_width() // 2, self.y - self.img.get_height() // 2, self.img.get_width(), self.img.get_height())
 
     def __draw__(self):
         self.rect = sys.window.screen.blit(self.img, self.getRect())
 
 
 class emptyimage(image):
     """An empty image."""
```

