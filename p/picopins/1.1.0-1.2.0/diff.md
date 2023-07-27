# Comparing `tmp/picopins-1.1.0.tar.gz` & `tmp/picopins-1.2.0.tar.gz`

## Comparing `picopins-1.1.0.tar` & `picopins-1.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 picopins-1.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 picopins-1.1.0/Makefile
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 picopins-1.1.0/README.md
--rwxr-xr-x   0        0        0     2071 2020-02-02 00:00:00.000000 picopins-1.1.0/check.sh
--rw-r--r--   0        0        0    34361 2020-02-02 00:00:00.000000 picopins-1.1.0/example.png
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 picopins-1.1.0/requirements-dev.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 picopins-1.1.0/requirements.txt
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 picopins-1.1.0/tox.ini
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 picopins-1.1.0/picopins/__init__.py
--rwxr-xr-x   0        0        0     9475 2020-02-02 00:00:00.000000 picopins-1.1.0/picopins/__main__.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 picopins-1.1.0/.gitignore
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 picopins-1.1.0/LICENSE
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 picopins-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     4215 2020-02-02 00:00:00.000000 picopins-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 picopins-1.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 picopins-1.2.0/Makefile
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 picopins-1.2.0/README.md
+-rwxr-xr-x   0        0        0     2071 2020-02-02 00:00:00.000000 picopins-1.2.0/check.sh
+-rw-r--r--   0        0        0    34361 2020-02-02 00:00:00.000000 picopins-1.2.0/example.png
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 picopins-1.2.0/requirements-dev.txt
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 picopins-1.2.0/requirements.txt
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 picopins-1.2.0/tox.ini
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 picopins-1.2.0/picopins/__init__.py
+-rwxr-xr-x   0        0        0     9918 2020-02-02 00:00:00.000000 picopins-1.2.0/picopins/__main__.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 picopins-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 picopins-1.2.0/LICENSE
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 picopins-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4335 2020-02-02 00:00:00.000000 picopins-1.2.0/PKG-INFO
```

### Comparing `picopins-1.1.0/Makefile` & `picopins-1.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `picopins-1.1.0/README.md` & `picopins-1.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,14 @@
        picopins      - basic GPIO pinout
 ```
 
 # Installing
 
 * Just run `python3 -m pip install picopins`
 
-# Achknowledgements
+# Acknowledgements
 
 This project was inspired by GPIO Zero's command-line pinout - https://github.com/gpiozero/gpiozero
 
 It somehow wasn't inspired by Raspberry Pi Spy's "picopins" which came first and solves this same problem in bash - https://www.raspberrypi-spy.co.uk/2022/12/pi-pico-pinout-display-on-the-command-line/
 
-Like RPi Spy's picopins it started as a GitHub gist, you can find the history here - https://gist.github.com/Gadgetoid/192af85a3eb05d4a6ac1db076c4ef118/revisions
+Like RPi Spy's picopins it started as a GitHub gist, you can find the history here - https://gist.github.com/Gadgetoid/192af85a3eb05d4a6ac1db076c4ef118/revisions
```

### Comparing `picopins-1.1.0/check.sh` & `picopins-1.2.0/check.sh`

 * *Files identical despite different names*

### Comparing `picopins-1.1.0/example.png` & `picopins-1.2.0/example.png`

 * *Files identical despite different names*

### Comparing `picopins-1.1.0/picopins/__main__.py` & `picopins-1.2.0/picopins/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/bin/env python3
 import re
 import sys
 
-from rich import print
+import rich
 from rich.panel import Panel
 from rich.table import Table
 
 """
 picopins, by @gadgetoid
 
 Support me:
@@ -14,17 +14,17 @@
 https://github.com/sponsors/Gadgetoid
 https://www.patreon.com/gadgetoid
 
 Shout-out to Raspberry Pi Spy for having almost this exact idea first:
 https://www.raspberrypi-spy.co.uk/2022/12/pi-pico-pinout-display-on-the-command-line/
 """
 
-__version__ = '1.1.0'
+__version__ = '1.2.0'
 
-PINOUT = [[col for col in line.split("|")] for line in """
+PINOUT = [line.split("|") for line in """
       |         |        |        |      |  |     ┏━━━━━┓     |  |          |        |        |         |
       |         |        |        |      |  |┏━━━━┫     ┣━━━━┓|  |          |        |        |         |
 PWM0 A|UART0 TX |I2C0 SDA|SPI0 RX |GP0   |1 |┃◎   ┗━━━━━┛   ◎┃|40|VBUS      |        |        |         |
 PWM0 B|UART0 RX |I2C0 SCL|SPI0 CSn|GP1   |2 |┃◎ ▩           ◎┃|39|VSYS      |        |        |         |
       |         |        |        |Ground|3 |┃▣ └─GP25      ▣┃|38|Ground    |        |        |         |
 PWM1 A|UART0 CTS|I2C1 SDA|SPI0 SCK|GP2   |4 |┃◎  ▒▒▒        ◎┃|37|3v3 En    |        |        |         |
 PWM1 B|UART0 RTS|I2C1 SCL|SPI0 TX |GP3   |5 |┃◎  ▒▒▒        ◎┃|36|3v3 Out   |        |        |         |
@@ -74,15 +74,15 @@
     "highlight": "bold #dc322f on white",
     "highlight_row": "bold {fg} on #444444"
 }
 
 
 def usage(error=None):
     error = f"\n[red]Error: {error}[/]\n" if error else ""
-    print(f"""
+    rich.print(f"""
 [#859900]picopins[/] [#2aa198]v{__version__}[/] - a beautiful GPIO pinout and pin function guide for the Raspberry Pi Pico
 {error}
 usage: picopins [--...] [--all] or {{{",".join(COLS[2:])}}} [--find <text>]
        --pins          - show physical pin numbers
        --all or {{{",".join(COLS[2:])}}} - pick list of interfaces to show
        --hide-gpio     - hide GPIO pins
        --light         - melt your eyeballs
@@ -156,82 +156,95 @@
         yield pin + " "
     yield " " + DIAGRAM[row]
     # We can't reverse a generator
     for pin in reversed(list(build_pins(RIGHT_PINS[row], show_indexes, highlight))):
         yield " " + pin
 
 
-def valid_label(label):
-    if label not in COLS[2:]:
-        usage(f"Invalid interface \"{label}\".")
-    return label
-
-
-def main():
-    if "--help" in sys.argv:
-        usage()
-
-    opts_all = "--all" in sys.argv
-    opts_pins = "--pins" in sys.argv
-    opts_hide_gpio = "--hide-gpio" in sys.argv
-    opts_light_mode = "--light" in sys.argv
-    opts_blink = "--blink" in sys.argv
-    opts_find = None
-
-    if "--find" in sys.argv:
-        index = sys.argv.index("--find") + 1
-        opts_find = sys.argv[index]
-        del sys.argv[index]
-
-    # Assume any non -- args are labels
-    opts_show = [valid_label(arg) for arg in sys.argv[1:] if not arg.startswith("--")]
-
-    if opts_show == [] and opts_all:
-        opts_show = COLS[2:]
-    elif opts_all:
-        usage("Please use either --all or a list of interfaces.")
-
+def picopins(opts):
     show_indexes = []
     grid = Table.grid(expand=True)
 
-    for label in reversed(opts_show):
+    for label in reversed(opts.show):
         grid.add_column(justify="left", style=THEME[label], no_wrap=True)
         show_indexes.append(COLS.index(label))
 
-    if not opts_hide_gpio:
+    if opts.show_gpio:
         grid.add_column(justify="right", style=THEME["gpio"], no_wrap=True)
         show_indexes.append(COL_GPIO)
 
-    if opts_pins:
+    if opts.show_pins:
         grid.add_column(justify="right", style=THEME["pins"], no_wrap=True)
         show_indexes.append(COL_PIN_NUMS)
 
     grid.add_column(no_wrap=True, style=THEME["diagram"])
 
-    if opts_pins:
+    if opts.show_pins:
         grid.add_column(justify="left", style=THEME["pins"], no_wrap=True)
 
-    if not opts_hide_gpio:
+    if opts.show_gpio:
         grid.add_column(justify="left", style=THEME["gpio"], no_wrap=True)
 
-    for label in opts_show:
+    for label in opts.show:
         grid.add_column(justify="left", style=THEME[label], no_wrap=True)
 
-    if opts_blink:
+    if search("GP25 LED", opts.find):
         DIAGRAM[LED_ROW] = DIAGRAM[LED_ROW].replace("▩", "[blink red]▩[/]")
+        DIAGRAM[LED_ROW + 1] = DIAGRAM[LED_ROW + 1].replace("GP25", styled("GP25", "highlight"))
 
     for i in range(ROWS):
-        grid.add_row(*build_row(i, show_indexes, highlight=opts_find))
+        grid.add_row(*build_row(i, show_indexes, highlight=opts.find))
 
     layout = Table.grid(expand=True)
     layout.add_row(grid)
     layout.add_row("@gadgetoid\nhttps://pico.pinout.xyz")
 
-    print(Panel(
+    return Panel(
         layout,
         title="Raspberry Pi Pico Pinout",
         expand=False,
-        style=THEME["panel_light"] if opts_light_mode else THEME["panel"]))
+        style=THEME["panel_light"] if opts.light_mode else THEME["panel"])
+
+
+class Options():
+    def __init__(self, argv):
+        argv.pop(0)
+
+        if "--help" in argv:
+            usage()
+
+        if "--version" in argv:
+            print(f"{__version__}")
+            sys.exit(0)
+
+        self.all = "--all" in argv
+        self.show_pins = "--pins" in argv
+        self.show_gpio = "--hide-gpio" not in argv
+        self.light_mode = "--light" in argv
+        self.find = None
+
+        if "--find" in argv:
+            index = argv.index("--find") + 1
+            if index >= len(argv) or argv[index].startswith("--"):
+                usage("--find needs something to find.")
+            self.find = argv.pop(index)
+
+        # Assume any non -- args are labels
+        self.show = [self.valid_label(arg) for arg in argv if not arg.startswith("--")]
+
+        if self.show == [] and self.all:
+            self.show = COLS[2:]
+        elif self.all:
+            usage("Please use either --all or a list of interfaces.")
+
+    def valid_label(self, label):
+        if label not in COLS[2:]:
+            usage(f"Invalid interface \"{label}\".")
+        return label
+
+
+def main():
+    rich.print(picopins(Options(sys.argv)))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `picopins-1.1.0/LICENSE` & `picopins-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `picopins-1.1.0/pyproject.toml` & `picopins-1.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Software Development",
     "Topic :: System :: Hardware",
 ]
-dependencies = ["rich"]
+dependencies = ["rich>=13.3.5"]
 
 [project.urls]
 GitHub = "https://www.github.com/pinout-xyz/picopins"
 Homepage = "https://pico.pinout.xyz"
 
 [project.scripts]
 picopins = "picopins.__main__:main"
```

### Comparing `picopins-1.1.0/PKG-INFO` & `picopins-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picopins
-Version: 1.1.0
+Version: 1.2.0
 Summary: A command-line pinout for the Raspberry Pi Pico W
 Project-URL: GitHub, https://www.github.com/pinout-xyz/picopins
 Project-URL: Homepage, https://pico.pinout.xyz
 Author-email: Philip Howard <pinout@gadgetoid.com>
 Maintainer-email: Philip Howard <pinout@gadgetoid.com>
 License: MIT License
         
@@ -39,15 +39,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: System :: Hardware
 Requires-Python: >=3.7
-Requires-Dist: rich
+Requires-Dist: rich>=13.3.5
 Description-Content-Type: text/markdown
 
 # Raspberry Pi Pico GPIO Pinout
 
 A beautiful GPIO pinout and pin function guide for the Raspberry Pi Pico.
 
 ![Example image](https://raw.githubusercontent.com/pinout-xyz/picopins/main/example.png)
@@ -69,23 +69,30 @@
        picopins      - basic GPIO pinout
 ```
 
 # Installing
 
 * Just run `python3 -m pip install picopins`
 
-# Achknowledgements
+# Acknowledgements
 
 This project was inspired by GPIO Zero's command-line pinout - https://github.com/gpiozero/gpiozero
 
 It somehow wasn't inspired by Raspberry Pi Spy's "picopins" which came first and solves this same problem in bash - https://www.raspberrypi-spy.co.uk/2022/12/pi-pico-pinout-display-on-the-command-line/
 
 Like RPi Spy's picopins it started as a GitHub gist, you can find the history here - https://gist.github.com/Gadgetoid/192af85a3eb05d4a6ac1db076c4ef118/revisions
+
 # Changelog
 
+1.2.0
+-----
+
+* Highlight LED if `--find GP25` or `--find LED`
+* Refactor options and add a `--version` command
+
 1.1.0
 -----
 
 * Highlight GPIO label if `--find` matches a hidden label
 * Add regex support to `--find`
 * Rewrite render flow to make it less hacky
 * Light mode is back! `--light`
```

