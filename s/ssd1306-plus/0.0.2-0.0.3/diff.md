# Comparing `tmp/ssd1306_plus-0.0.2.tar.gz` & `tmp/ssd1306_plus-0.0.3.tar.gz`

## Comparing `ssd1306_plus-0.0.2.tar` & `ssd1306_plus-0.0.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 ssd1306_plus-0.0.2/src/ssd1306_plus.py
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 ssd1306_plus-0.0.2/LICENSE
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 ssd1306_plus-0.0.2/README.md
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 ssd1306_plus-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 ssd1306_plus-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 ssd1306_plus-0.0.3/ssd1306_plus.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 ssd1306_plus-0.0.3/LICENSE
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 ssd1306_plus-0.0.3/README.md
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 ssd1306_plus-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 ssd1306_plus-0.0.3/PKG-INFO
```

### Comparing `ssd1306_plus-0.0.2/src/ssd1306_plus.py` & `ssd1306_plus-0.0.3/ssd1306_plus.py`

 * *Files identical despite different names*

### Comparing `ssd1306_plus-0.0.2/LICENSE` & `ssd1306_plus-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ssd1306_plus-0.0.2/PKG-INFO` & `ssd1306_plus-0.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: ssd1306_plus
-Version: 0.0.2
+Version: 0.0.3
 Summary: Augments the SSD1306_I2C MicroPython library with high-level functions
 Author-email: Code Cadets <codecadets@cgs.act.edu.au>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Description-Content-Type: text/markdown
 
 # SSD1306_PLUS
 
 For MicroPython only.
 
+Added `draw_sprite` function to ssd1306_I2C library 
+
 ```python
 from machine import I2C
 i2c = I2C(0,sda=Pin(0), scl=Pin(1), freq=400000)
 oled = SSD1306_PLUS(128, 64, i2c)
 
 star = '''
 .#.
```

