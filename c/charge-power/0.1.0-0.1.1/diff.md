# Comparing `tmp/charge_power-0.1.0.tar.gz` & `tmp/charge_power-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "charge_power-0.1.0.tar", max compression
+gzip compressed data, was "charge_power-0.1.1.tar", max compression
```

## Comparing `charge_power-0.1.0.tar` & `charge_power-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0       77 2023-07-07 09:35:28.476120 charge_power-0.1.0/README.md
--rw-r--r--   0        0        0      186 2023-07-10 10:32:49.772006 charge_power-0.1.0/charge_power/__init__.py
--rw-r--r--   0        0        0     3497 2023-07-10 15:52:00.740412 charge_power-0.1.0/charge_power/__main__.py
--rw-r--r--   0        0        0      109 2023-07-10 15:05:17.960326 charge_power-0.1.0/charge_power/charge/__init__.py
--rw-r--r--   0        0        0     3570 2023-07-10 15:39:51.264389 charge_power-0.1.0/charge_power/charge/print_charge.py
--rw-r--r--   0        0        0      954 2023-07-10 15:40:33.620391 charge_power-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      769 1970-01-01 00:00:00.000000 charge_power-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-20 09:46:31.038948 charge_power-0.1.1/LICENSE
+-rw-r--r--   0        0        0      661 2023-07-20 09:52:40.618075 charge_power-0.1.1/README.md
+-rw-r--r--   0        0        0      122 2023-07-27 16:51:41.429801 charge_power-0.1.1/charge_power/__init__.py
+-rw-r--r--   0        0        0     3645 2023-07-27 16:56:31.480213 charge_power-0.1.1/charge_power/__main__.py
+-rw-r--r--   0        0        0      109 2023-07-20 09:52:40.618075 charge_power-0.1.1/charge_power/charge/__init__.py
+-rw-r--r--   0        0        0     3581 2023-07-27 16:49:28.931089 charge_power-0.1.1/charge_power/charge/print_charge.py
+-rw-r--r--   0        0        0     1125 2023-07-27 16:54:39.463988 charge_power-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1568 1970-01-01 00:00:00.000000 charge_power-0.1.1/PKG-INFO
```

### Comparing `charge_power-0.1.0/charge_power/__main__.py` & `charge_power-0.1.1/charge_power/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,31 @@
-"""
-Print current wattage of charge/discharge
-"""
+"""Print current wattage of charge/discharge"""
+from __future__ import annotations
+
 import itertools
 import os
 import sys
 from pathlib import Path
 
 import click
 from rich.console import Console
 
+from charge_power import __version__ as version
 from charge_power.charge import print_battery_charge
 
 
 _CHARGE_COEFF = 0.00001139850942569049  # coefficient to multiply current_charge value to get Watts
 
 
 @click.command("print_wattage")
-@click.option("--delay", "-d", type=int, default=10, help="Delay in seconds between measurements", show_default=True)
-@click.option("--number", "-n", type=int, default=None, help="Delay in seconds between measurements", show_default=True)
+@click.version_option(version)
+@click.option("--delay", "-d", type=int, default=30, help="Delay between measurements in seconds", show_default=True)
+@click.option(
+    "--number", "-n", type=int, default=None, help="Number of measurements before stop", show_default="(unlimited)"
+)
 @click.option("--log-file", "-l", type=click.Path(dir_okay=False), default=None, help="Path to a file to log output")
 @click.argument(
     "battery_path", type=click.Path(exists=True, file_okay=False), default=None, metavar="BATTERY_PATH", required=False
 )
 def main(delay: int, number: int | None, log_file: str | None, battery_path: str | None):
     """
     Show power usage of the given battery.
@@ -52,24 +56,25 @@
 
     logfile = None
     current_charge = get_charge()
     if log_file is not None:
         try:
             logfile = open(log_file, "a", encoding="utf-8")  # pylint: disable=consider-using-with
             print(
-                f"Starting to print charge change (delay={delay}, number={number}). Current charge is {current_charge:.2f}W",
+                f"Starting to print charge change (delay={delay}, number={number})."
+                f" Current charge is {current_charge:.2f}Wh",
                 file=logfile,
             )
         except Exception as exc:  # pylint: disable=broad-except
             console.print(f"[red]Could not open file [i]{log_file}[/i] to log data[/red]: {exc!r}")
             sys.exit(1)
 
     console.print(
         f"Starting to print charge change [dim](delay={delay}, number={number})[/dim]."
-        f" Current charge is [green]{current_charge:.2f}[/green]W"
+        f" Current charge is [green]{current_charge:.2f}[/green]Wh"
     )
     try:
         print_battery_charge(get_charge, full_wattage, delay, rng, console, logfile)
     except KeyboardInterrupt:
         print("Finishing by Ctrl+C hit")
     finally:
         if logfile is not None:
@@ -77,10 +82,10 @@
                 logfile.close()
             except Exception as exc:  # pylint: disable=broad-except
                 console.print(f"[red]Could not close log file [i]{log_file}[/red]: {exc!r}")
 
 
 if __name__ == "__main__":
     if os.name != "posix":
-        print("This script works only with linux systems")
+        print("This utility works only with linux systems")
         sys.exit(1)
     main()  # pylint: disable=no-value-for-parameter
```

### Comparing `charge_power-0.1.0/charge_power/charge/print_charge.py` & `charge_power-0.1.1/charge_power/charge/print_charge.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,56 @@
 """Function used to print battery charge change is defined here."""
+from __future__ import annotations
+
 import datetime
 import time
 from typing import Callable, Iterable, NoReturn, TextIO
 
 from rich.console import Console
 
 
 def _prepare_print(  # pylint: disable=too-many-arguments
     iteration: int,
     old_time_ns: int,
     old_value: float,
     new_time_ns: int,
     new_value: float,
-    full_wattage: float,
+    full_capacity: float,
 ) -> str:
     """Prepare concrete measurement of wattage difference message for rich.Console print"""
     real_delay = new_time_ns - old_time_ns
     delay_seconds = round(real_delay / 1_000_000_000)
     difference = new_value - old_value
 
     per_hour = difference * 1_000_000_000 * 3600 / real_delay
     if difference == 0:
         return (
             f"{datetime.datetime.now().strftime('%m-%d %H:%M:%S')} ({iteration:3}):    stable"
-            f" [cyan]{0.0}[/cyan]W per hour: [green]{new_value:5.2f}[/green]W of"
-            f" {full_wattage:.2f}W ({new_value / full_wattage * 100:.1f}%)"
+            f" [cyan]{0.0}[/cyan]W: [green]{new_value:5.2f}[/green]Wh of"
+            f" {full_capacity:.2f}Wh ({new_value / full_capacity * 100:.1f}%)"
         )
-    time_left = (full_wattage - new_value) / per_hour * 60 if difference > 0 else (new_value) / -per_hour * 60
+    time_left = (full_capacity - new_value) / per_hour * 60 if difference > 0 else (new_value) / -per_hour * 60
     time_left_str = (
         f"{time_left:4.1f} minutes" if time_left < 60 else f"{time_left // 60:.0f}:{time_left % 60:02.0f} hours"
     )
     if difference > 0:
         return (
             f"{datetime.datetime.now().strftime('%m-%d %H:%M:%S')} ({iteration:3}):    charge"
-            f" {difference * 1000:7.2f}mW per {delay_seconds} seconds"
-            f" ([green]{per_hour:7.2f}[/green]W per hour):"
-            f" [yellow]{old_value:5.2f}[/yellow]W -> [green]{new_value:5.2f}[/green]W of"
-            f" {full_wattage:.2f}W ({new_value / full_wattage * 100:.1f}%,"
-            f" [i]{time_left_str} minutes to full[/i])"
+            f" {difference * 1000:7.2f}mWh per {delay_seconds} seconds"
+            f" ([green]{per_hour:7.2f}[/green]W):"
+            f" [yellow]{old_value:5.2f}[/yellow]Wh -> [green]{new_value:5.2f}[/green]Wh of"
+            f" {full_capacity:.2f}Wh ({new_value / full_capacity * 100:.1f}%,"
+            f" [i]{time_left_str} to full[/i])"
         )
     return (
         f"{datetime.datetime.now().strftime('%m-%d %H:%M:%S')} ({iteration:3}): discharge"
-        f" {difference * 1000:7.2f}mW per {delay_seconds} seconds ([red]{per_hour:7.2f}[/red]W per hour):"
-        f" [yellow]{old_value:5.2f}[/yellow]W -> [red]{new_value:5.2f}[/red]W of"
-        f" {full_wattage:.2f}W ({new_value / full_wattage * 100:.1f}%,"
-        f" [i]{time_left_str} minutes to zero[/i])"
+        f" {difference * 1000:7.2f}mWh per {delay_seconds} seconds ([red]{per_hour:7.2f}[/red]W):"
+        f" [yellow]{old_value:5.2f}[/yellow]Wh -> [red]{new_value:5.2f}[/red]Wh of"
+        f" {full_capacity:.2f}Wh ({new_value / full_capacity * 100:.1f}%,"
+        f" [i]{time_left_str} to zero[/i])"
     )
 
 
 def print_battery_charge(  # pylint: disable=too-many-arguments
     get_charge: Callable[[], int],
     full_wattage: float,
     delay_seconds: int,
```

### Comparing `charge_power-0.1.0/pyproject.toml` & `charge_power-0.1.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,24 @@
 [tool.poetry]
 name = "charge-power"
-version = "0.1.0"
+version = "0.1.1"
 description = "Small utility to track current charge/discharge wattage based on system sensors (Linux only)"
 authors = ["Aleksei Sokol <kanootoko@gmail.com>"]
-urls = { repository = "https://github.com/kanootoko/charge_power" }
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "charge_power" }]
+repository = "https://github.com/kanootoko/charge-power"
+
+classifiers = [
+    "Operating System :: POSIX :: Linux",
+    "Topic :: System :: Hardware",
+]
+
+[tool.poetry.urls]
+"Bug tracker" = "https://github.com/kanootoko/charge-power/issues"
 
 
 [tool.poetry.dependencies]
 python = "^3.9"
 rich = "^13.4.2"
 click = "^8.1.4"
 
@@ -25,15 +33,15 @@
 charge-power = "charge_power.__main__:main"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
-target-version = ['py310']
+target-version = ['py39']
 line_length = 120
 
 [tool.pylint.format]
 max-line-length = 120
 
 [tool.isort]
 known_local_folder = "charge_power"
```

