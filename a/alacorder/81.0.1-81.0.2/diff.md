# Comparing `tmp/alacorder-81.0.1.tar.gz` & `tmp/alacorder-81.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-81.0.1.tar", max compression
+gzip compressed data, was "alacorder-81.0.2.tar", max compression
```

## Comparing `alacorder-81.0.1.tar` & `alacorder-81.0.2.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     4865 2023-07-25 18:33:12.479611 alacorder-81.0.1/README.md
--rw-r--r--   0        0        0     6148 2023-07-25 19:24:50.768113 alacorder-81.0.1/alacorder/.DS_Store
--rw-r--r--   0        0        0       19 2023-07-25 19:20:19.054678 alacorder-81.0.1/alacorder/__init__.py
--rw-r--r--   0        0        0       59 2023-07-25 19:23:49.408885 alacorder-81.0.1/alacorder/__main__.py
--rw-r--r--   0        0        0   198912 2023-07-25 18:51:12.632257 alacorder-81.0.1/alacorder/alac.py
--rw-r--r--   0        0        0      557 2023-07-25 18:50:57.676450 alacorder-81.0.1/pyproject.toml
--rw-r--r--   0        0        0     5617 1970-01-01 00:00:00.000000 alacorder-81.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-18 14:01:34.633926 alacorder-81.0.2/LICENSE
+-rw-r--r--   0        0        0     4865 2023-07-25 18:33:12.479611 alacorder-81.0.2/README.md
+-rw-r--r--   0        0        0     6148 2023-07-25 19:27:15.912541 alacorder-81.0.2/alacorder/.DS_Store
+-rw-r--r--   0        0        0       19 2023-07-25 19:20:19.054678 alacorder-81.0.2/alacorder/__init__.py
+-rw-r--r--   0        0        0       59 2023-07-25 19:23:49.408885 alacorder-81.0.2/alacorder/__main__.py
+-rw-r--r--   0        0        0   183002 2023-07-27 21:52:57.145527 alacorder-81.0.2/alacorder/alac.py
+-rw-r--r--   0        0        0      557 2023-07-27 21:53:48.864160 alacorder-81.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5617 1970-01-01 00:00:00.000000 alacorder-81.0.2/PKG-INFO
```

### Comparing `alacorder-81.0.1/README.md` & `alacorder-81.0.2/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-81.0.1/alacorder/.DS_Store` & `alacorder-81.0.2/alacorder/.DS_Store`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 00000000: 0000 0001 4275 6431 0000 1000 0000 0800  ....Bud1........
 00000010: 0000 1000 0000 0108 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0002 0000 0000 0000 0004  ................
+00000040: 0000 0000 0000 0002 0000 0000 0000 0003  ................
 00000050: 0000 0001 0000 1000 0069 0074 005f 005f  .........i.t._._
 00000060: 002e 0070 0000 0000 0000 0000 0000 0000  ...p............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000100: 0000 0000 0000 0000 0000 0004 0000 000b  ................
+00000100: 0000 0000 0000 0000 0000 0003 0000 000b  ................
 00000110: 005f 005f 0069 006e 0069 0074 005f 005f  ._._.i.n.i.t._._
 00000120: 002e 0070 0079 496c 6f63 626c 6f62 0000  ...p.yIlocblob..
 00000130: 0010 0000 0041 0000 002e ffff ffff ffff  .....A..........
 00000140: 0000 0000 000b 005f 005f 006d 0061 0069  ......._._.m.a.i
 00000150: 006e 005f 005f 002e 0070 0079 496c 6f63  .n._._...p.yIloc
 00000160: 626c 6f62 0000 0010 0000 00af 0000 002e  blob............
-00000170: ffff ffff ffff 0000 0000 000b 005f 005f  ............._._
-00000180: 0070 0079 0063 0061 0063 0068 0065 005f  .p.y.c.a.c.h.e._
-00000190: 005f 496c 6f63 626c 6f62 0000 0010 0000  ._Ilocblob......
-000001a0: 018b 0000 002e ffff ffff ffff 0000 0000  ................
-000001b0: 0007 0061 006c 0061 0063 002e 0070 0079  ...a.l.a.c...p.y
-000001c0: 496c 6f63 626c 6f62 0000 0010 0000 0119  Ilocblob........
-000001d0: 0000 002f ffff ffff ffff 0000 0000 0000  .../............
+00000170: ffff ffff ffff 0000 0000 0007 0061 006c  .............a.l
+00000180: 0061 0063 002e 0070 0079 496c 6f63 626c  .a.c...p.yIlocbl
+00000190: 6f62 0000 0010 0000 0119 0000 002f ffff  ob.........../..
+000001a0: ffff ffff 0000 0000 0000 0000 0000 0000  ................
+000001b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000230: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000240: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `alacorder-81.0.1/alacorder/alac.py` & `alacorder-81.0.2/alacorder/alac.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ┣┫┃ ┣┫┃ ┃┃┣┫┃┃┣ ┣┫
 ┛┗┗┛┛┗┗┛┗┛┛┗┻┛┗┛┛┗
 (c) 2023 Sam Robson
 
 Dependencies: Python 3.9+, Google Chrome, brotli 1.0.9+, polars 0.18.1+, pymupdf 1.21.1+, rich 13.3.3+, selenium 4.8.3+, typer 0.9.0+, xlsx2csv 0.8.1+, xlsxwriter 3.0.9+
 """
 
-__version__ = "81.0.1"
+__version__ = "81.0.2"
 
 import os
 import re
 import glob
 import time
 import typer
 from typing_extensions import Annotated
@@ -26,26 +26,25 @@
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.ui import Select
 from selenium.webdriver.support.wait import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
 
 pl.Config.set_tbl_rows(20)
 pl.Config.set_fmt_str_lengths(100)
-pl.Config.set_tbl_width_chars(100)
 pl.Config.set_tbl_formatting("NOTHING")
 pl.Config.set_tbl_dataframe_shape_below(True)
 pl.Config.set_tbl_hide_column_data_types(True)
 
 console = Console()
 progress_bar = Progress(*Progress.get_default_columns(), MofNCompleteColumn())
 app = typer.Typer(help="Alacorder collects case detail PDFs from Alacourt.com and processes them into data tables suitable for research purposes.", no_args_is_help=True, pretty_exceptions_show_locals=False, add_completion=False)
 
 def write(output: dict, path: str, log: bool = False):
     """
-    Write each value in {'name': pl.DataFrame} to path. (Supports .xls, .xlsx, .csv, .json, and .parquet)
+    Write each value in `output` dict {'name': pl.DataFrame} to path. If exporting multiple tables, extension must be .xls or .xlsx. Otherwise, write() supports .xls, .xlsx, .csv, .json, and .parquet.
     """
     def _write(output: dict, path: str):
         if isinstance(output, pl.DataFrame): # convert to dict
             if "AllPagesTextNoNewLine" in output.columns:
                 output = output.select(pl.exclude("AllPagesTextNoNewLine"))
             output = {'table': output}
         ext = os.path.splitext(path)[1]
@@ -166,15 +165,15 @@
                 pl.col("AllPagesText").str.replace_all(r"\n"," ").alias("AllPagesTextNoNewLine")
             )
     return output
 
 class AlacourtDriver():
     
     # config
-    def __init__(self, dirpath=None, headless=True):
+    def __init__(self, dirpath=None, headless=True, cID=None, uID=None, pwd=None):
         opt = webdriver.ChromeOptions()
         if headless:
             opt.add_argument("--headless=new")
         if dirpath != None:
             opt.add_experimental_option(
                 "prefs",
                 {
@@ -196,31 +195,46 @@
         if dirpath != None:
             self.dirpath = os.path.abspath(dirpath)
         else:
             self.dirpath = None
         self.headless = headless
         with console.status("Starting WebDriver (requires Google Chrome)..."):
             self.driver = webdriver.Chrome(options=opt)
-        self.queue = None
+        self.party_search_queue = None
         self.case_number_queue = None
         self.output = None
+        self.cID = cID
+        self.uID = uID
+        self.pwd = pwd
+        if cID != None and uID != None and pwd != None:
+            self.login(cID, uID, pwd)
     
-    def login(self, cID, uID, pwd) -> None:
+    def login(self, cID=None, uID=None, pwd=None) -> None:
         """
         Login to Alacourt using provided credentials.
         """
+        if cID != None:
+            self.cID = cID
+        if uID != None:
+            self.uID = uID
+        if pwd != None:
+            self.pwd = pwd
+
+        if self.cID == None or self.uID == None or self.pwd == None:
+            raise Exception("Must enter Alacourt credentials to login.")
+
         with console.status("Logging in to Alacourt..."):
             self.driver.get("https://v2.alacourt.com")
             cID_box = self.driver.find_element(by=By.ID, value="ContentPlaceHolder_txtCusid")
             uID_box = self.driver.find_element(by=By.ID, value="ContentPlaceHolder_txtUserId")
             pwd_box = self.driver.find_element(by=By.ID, value="ContentPlaceHolder_txtPassword")
             login_button = self.driver.find_element(by=By.ID, value="ContentPlaceHolder_btLogin")
-            cID_box.send_keys(cID)
-            uID_box.send_keys(uID)
-            pwd_box.send_keys(pwd)
+            cID_box.send_keys(self.cID)
+            uID_box.send_keys(self.uID)
+            pwd_box.send_keys(self.pwd)
             login_button.click()
             continue_button = self.driver.find_elements(by=By.ID, value="ContentPlaceHolder_btnContinueLogin")
             if len(continue_button) > 0:
                 continue_button[0].click()
             try:
                 WebDriverWait(self.driver, 5).until(EC.visibility_of_element_located((By.ID, "btnLogOff")))
                 return True
@@ -230,44 +244,44 @@
     # party search
     def set_party_search_queue(self, queue) -> None:
         """
         Set path to Party Search queue spreadsheet.
         """
         if isinstance(queue, pl.DataFrame):
             self.queue_path = None
-            self.queue = queue
+            self.party_search_queue = queue
         if isinstance(queue, str):
             if os.path.isfile(queue):
                 self.queue_path = queue
-                self.queue = read(queue)
+                self.party_search_queue = read(queue)
             else:
                 raise Exception("Could not read input.")
         for col in ["Retrieved", "Timestamp", "Case Count"]:
-            if col not in self.queue.columns:
-                self.queue = self.queue.with_columns(
+            if col not in self.party_search_queue.columns:
+                self.party_search_queue = self.party_search_queue.with_columns(
                     pl.lit("").alias(col)
                 )
         pscols = ["NAME", "PARTY_TYPE", "SSN", "DOB", "COUNTY", "DIVISION", "CASE_YEAR", "NO_RECORDS", "FILED_BEFORE", "FILED_AFTER"]
         col_dict = {}
-        for col in self.queue.columns:
+        for col in self.party_search_queue.columns:
             d = {re.sub(" ", "_", col.upper()): col}
             col_dict.update(d)
         for key in col_dict:
             if key in pscols:
-                self.queue = self.queue.with_columns(
+                self.party_search_queue = self.party_search_queue.with_columns(
                     pl.col(col_dict[key]).alias("TEMP_" + key)
                 )
         temp_pscols = ["TEMP_" + col for col in pscols]
         for col in temp_pscols:
-            if col not in self.queue.columns:
-                self.queue = self.queue.with_columns(
+            if col not in self.party_search_queue.columns:
+                self.party_search_queue = self.party_search_queue.with_columns(
                     pl.lit("").alias(col)
                 )
-        for col in self.queue.columns:
-            self.queue = self.queue.with_columns(
+        for col in self.party_search_queue.columns:
+            self.party_search_queue = self.party_search_queue.with_columns(
                 pl.when(pl.col(col)==None).then('').otherwise(pl.col(col)).alias(col)
             )
     
     def set_party_search_output(self, output_path) -> None:
         """
         Set path to Party Search output spreadsheet.
         """
@@ -281,15 +295,16 @@
         try:
             if "frmIndexSearchForm" not in self.driver.current_url:
                 self.driver.get("https://v2.alacourt.com/frmIndexSearchForm.aspx")
         except:
             self.driver.get("https://v2.alacourt.com/frmIndexSearchForm.aspx")
 
         if "frmlogin" in self.driver.current_url:
-            raise Exception("Must be logged into Alacourt before party searching.")
+            self.login()
+            self.driver.get("https://v2.alacourt.com/frmIndexSearchForm.aspx")
         
         # locators
         party_name_box = self.driver.find_element(by=By.NAME, value="ctl00$ContentPlaceHolder1$txtName")
         ssn_box = self.driver.find_element(by=By.NAME, value="ctl00$ContentPlaceHolder1$txtSSN")
         dob_box = self.driver.find_element(by=By.NAME, value="ctl00$ContentPlaceHolder1$txtDOB")
         plaintiffs_pt_select = self.driver.find_element(by=By.ID, value="ContentPlaceHolder1_rdlPartyType_0")
         defendants_pt_select = self.driver.find_element(by=By.ID, value="ContentPlaceHolder1_rdlPartyType_1")
@@ -392,36 +407,38 @@
             page_select = Select(self.driver.find_element(by=By.ID, value="ContentPlaceHolder1_dg_ddlPages"))
             page_select.select_by_visible_text(str(i))
             WebDriverWait(self.driver, 10).until(EC.staleness_of(table))
             table = self.driver.find_element(by=By.ID, value="ContentPlaceHolder1_dg")
             df = pl.concat([df, self.read_results_page()])
         return df   
     
-    def start_party_search_queue(self, queue=None, output_path=None, criminal_only=False) -> pl.DataFrame:
+    def start_party_search_queue(self, queue=None, output_path=None, criminal_only=False, verbose=False) -> pl.DataFrame:
         """
         From `queue`, conduct Party Search and record results tables to `output_path`.
         """
         if isinstance(queue, pl.DataFrame) or isinstance(queue, str):
             self.set_party_search_queue(queue)
-        elif self.queue == None:
+        elif self.party_search_queue == None:
             raise Exception("Must set queue to start.")
         if output_path != None:
             self.set_party_search_output(output_path)
         try:
             results_df = read(self.output)
             for col in results_df.columns:
                 results_df = results_df.with_columns(
                     pl.col(col).cast(pl.Utf8)
                 )
             print("Appending to existing table at output path.")
         except:
             results_df = pl.DataFrame()
         with progress_bar as p:
-            for i, r in enumerate(p.track(self.queue.rows(named=True), description="Party searching...")):
+            for i, r in enumerate(p.track(self.party_search_queue.rows(named=True), description="Party searching...")):
                 if r['Retrieved'] in ('', None):
+                    if verbose:
+                        p.console.log(f"#{i+1}: {r['TEMP_NAME']}")
                     self.party_search(
                         name=r['TEMP_NAME'],
                         party_type=r['TEMP_PARTY_TYPE'],
                         ssn=r['TEMP_SSN'],
                         dob=r['TEMP_DOB'],
                         county=r['TEMP_COUNTY'],
                         division=r['TEMP_DIVISION'],
@@ -434,24 +451,24 @@
                     df = self.read_all_results()
                     df = df.with_columns(pl.lit(r['TEMP_NAME']).alias("Search"))
                     for col in ["Retrieved", "Timestamp", "Destination"]:
                         if col in results_df.columns:
                             df = df.with_columns(pl.lit('').alias(col))
                     if df.shape[0] > 1:
                         results_df = pl.concat([results_df, df])
-                    self.queue[i, 'Retrieved'] = "Y"
-                    self.queue[i, 'Case Count'] = df.shape[0]
-                    self.queue[i, 'Timestamp'] = time.time()
+                    self.party_search_queue[i, 'Retrieved'] = "Y"
+                    self.party_search_queue[i, 'Case Count'] = df.shape[0]
+                    self.party_search_queue[i, 'Timestamp'] = time.time()
                     if self.queue_path != None and i % 10 == 0:
-                        write_queue = self.queue.select(pl.exclude("TEMP_NAME", "TEMP_PARTY_TYPE", "TEMP_SSN", "TEMP_DOB", "TEMP_COUNTY", "TEMP_DIVISION", "TEMP_CASE_YEAR", "TEMP_FILED_BEFORE", "TEMP_FILED_AFTER", "TEMP_NO_RECORDS"))
+                        write_queue = self.party_search_queue.select(pl.exclude("TEMP_NAME", "TEMP_PARTY_TYPE", "TEMP_SSN", "TEMP_DOB", "TEMP_COUNTY", "TEMP_DIVISION", "TEMP_CASE_YEAR", "TEMP_FILED_BEFORE", "TEMP_FILED_AFTER", "TEMP_NO_RECORDS"))
                         write({'queue': write_queue}, self.queue_path)
                     if self.output != None and i % 10 == 0:
                         write({'results': results_df}, self.output)
             if self.queue_path != None:
-                write_queue = self.queue.select(pl.exclude("TEMP_NAME", "TEMP_PARTY_TYPE", "TEMP_SSN", "TEMP_DOB", "TEMP_COUNTY", "TEMP_DIVISION", "TEMP_CASE_YEAR", "TEMP_FILED_BEFORE", "TEMP_FILED_AFTER", "TEMP_NO_RECORDS"))
+                write_queue = self.party_search_queue.select(pl.exclude("TEMP_NAME", "TEMP_PARTY_TYPE", "TEMP_SSN", "TEMP_DOB", "TEMP_COUNTY", "TEMP_DIVISION", "TEMP_CASE_YEAR", "TEMP_FILED_BEFORE", "TEMP_FILED_AFTER", "TEMP_NO_RECORDS"))
                 write({'queue': write_queue}, self.queue_path)
             if self.output != None:
                 write({'results': results_df}, self.output)
         return results_df
     
     # case number search
     def set_case_number_queue(self, queue) -> None:
@@ -474,15 +491,16 @@
     def case_number_search(self, case_number='', download=True) -> bool:
         """
         Use Alacourt Case Lookup to search for a case by number. If `download` is true, will also download case detail PDF. Returns False if case detail is unavailable.
         """
         self.driver.get("https://v2.alacourt.com/frmcaselookupform.aspx")
 
         if "frmlogin" in self.driver.current_url:
-            raise Exception("Must be logged into Alacourt before fetching cases.")
+            self.login()
+            self.driver.get("https://v2.alacourt.com/frmcaselookupform.aspx")
 
         county_select = self.driver.find_element(by=By.NAME, value="ctl00$ContentPlaceHolder1$ddlCounty")
         division_select = self.driver.find_element(by=By.NAME, value="ctl00$ContentPlaceHolder1$ddlDivision")
         case_year_select = self.driver.find_element(by=By.NAME, value="ctl00$ContentPlaceHolder1$ddlCaseYear")
         case_number_input = self.driver.find_element(by=By.NAME, value="ctl00$ContentPlaceHolder1$txtCaseNumber")
         case_extension_select = self.driver.find_element(by=By.NAME, value="ctl00$ContentPlaceHolder1$ddlExt")
         number_of_cases_select = self.driver.find_element(by=By.NAME, value="ctl00$ContentPlaceHolder1$ddlNumberOfCases")
@@ -498,15 +516,18 @@
         division_code = case_number[3:5]
         case_year = case_number[6:10]
         six_digit = case_number[11:17]
         if len(case_number) >= 20:
             extension = case_number[18:20]
         else:
             extension = "00"
-        county = cmap.filter(pl.col("CountyNumber")==county_number).select("Selection").to_series()[0]
+        try:
+            county = cmap.filter(pl.col("CountyNumber")==county_number).select("Selection").to_series()[0]
+        except:
+            return False
         division = dmap.filter(pl.col("Code")==division_code).select("Selection").to_series()[0]
         county_select.send_keys(county)
         division_select.send_keys(division)
         case_year_select.send_keys(case_year)
         case_number_input.send_keys(six_digit)
         search_button = self.driver.find_element(by=By.ID, value="searchButton")
         search_button.click()
@@ -519,22 +540,24 @@
                 except:
                     return False
                 self.driver.find_element(by=By.ID, value="ContentPlaceHolder1_lnkPrint").click()
                 WebDriverWait(self.driver, 10).until(EC.visibility_of_element_located((By.ID, "divPrintCase")))
                 self.driver.find_element(by=By.ID, value="btnPrintCase").click()
                 return True
 
-    def start_case_number_queue(self, queue=None):
+    def start_case_number_queue(self, queue=None, verbose=False):
         if isinstance(queue, pl.DataFrame) or isinstance(queue, str):
             self.set_case_number_queue(queue)
         elif self.case_number_queue == None:
             raise Exception("Must set queue to start.")
         with progress_bar as p:
             for i, r in enumerate(p.track(self.case_number_queue.rows(named=True), description="Fetching cases...")):
                 if r['Retrieved'] in ('', None):
+                    if verbose:
+                        p.console.log(f"#{i+1}: {r['CaseNumber']}")
                     if self.case_number_search(r['CaseNumber']):
                         self.case_number_queue[i, 'Retrieved'] = "Y"
                         self.case_number_queue[i, 'Timestamp'] = time.time()
                         self.case_number_queue[i, 'Destination'] = self.dirpath
                     else:
                         self.case_number_queue[i, 'Retrieved'] = "PDF Not Available"
                         self.case_number_queue[i, 'Timestamp'] = time.time()
@@ -785,15 +808,15 @@
                 pl.col("Name").str.extract(r'([A-Z]+)').alias("TEMP_LAST_NAME"),
                 pl.col("Name").str.extract(r' ([A-Z]+)').alias("TEMP_FIRST_NAME")
             ])
         for col in ["TEMP_LAST_NAME", "TEMP_FIRST_NAME", "TEMP_AIS"]:
             if col not in self.queue.columns:
                 self.queue = self.queue.with_columns(pl.lit('').alias(col))
 
-    def start_queue(self, queue=None, output_path=None):
+    def start_queue(self, queue=None, output_path=None, verbose=False):
         """
         ADOC Inmate Search for each in `queue`, and save results to `output_path`.
         """
         if isinstance(queue, pl.DataFrame) or isinstance(queue, str):
             self.set_queue(queue)
         elif self.queue == None:
             raise Exception("Must set queue to start.")
@@ -817,14 +840,16 @@
         except:
             inmate_details = pl.DataFrame()
             blue_tables = pl.DataFrame()
             black_tables = pl.DataFrame()
         with progress_bar as p:
             for i, r in enumerate(p.track(self.queue.rows(named=True), description="Searching ADOC...")):
                 if r['Retrieved'] in (None, ""):
+                    if verbose:
+                        p.console.log(f"#{i+1}: {r['TEMP_AIS']} {r['TEMP_FIRST_NAME']} {r['TEMP_LAST_NAME']}")
                     self.search(ais=r['TEMP_AIS'], first_name=r['TEMP_FIRST_NAME'], last_name=r['TEMP_LAST_NAME'])
                     if self.select_result(0):
                         results = self.read_results_page()
                         inmate_details = pl.concat([inmate_details, results['InmateDetails']])
                         blue_tables = pl.concat([blue_tables, results['BlueTables']])
                         black_tables = pl.concat([black_tables, results['BlackTables']])
                         self.queue[i, 'Retrieved'] = "Y"
@@ -861,15 +886,16 @@
             else:
                 raise Exception("Could not read input.")
         if isinstance(archive, pl.DataFrame):
             self.archive = read(archive)
             self.is_read = True
         self._cases = None
         self._fees = None
-        self._charges = None
+        self._filing_charges = None
+        self._disposition_charges = None
         self._sentences = None
         self._financial_history = None
         self._settings = None
         self._case_action_summary = None
         self._witnesses = None
         self._attorneys = None
         self._images = None
@@ -1607,379 +1633,232 @@
                     "Balance",
                     "AmtHold",
                 )
                 out = out.fill_null("")
                 out = out.drop_nulls("AmtDue")
             self._fees = out
             return self._fees
-    
-    def charges(self):
-        if isinstance(self._charges, pl.DataFrame):
-            return self._charges
+
+    def filing_charges(self):
+        if isinstance(self._filing_charges, pl.DataFrame):
+            return self._filing_charges
         else:
             if not self.is_read:
                 self.read()
-            with console.status("Parsing charges..."):
-                all_charges = self.archive.with_columns(
-                    [
-                        pl.col("AllPagesText")
+            with console.status("Parsing filing charges..."):
+                df = self.archive.select("CaseNumber", "AllPagesText")
+                df = df.select([
+                    pl.col("CaseNumber"),
+                    pl.col("AllPagesText").str.extract(r'(?s)Filing Charges(.+?)Disposition Charges').str.replace(r"\n\s*# Code Description Cite Type Description Category ID Class\s*\n\s*","").str.strip().alias("FilingCharges"),
+                    pl.col("AllPagesText")
                         .str.extract(
                             r"(?:VS\.|V\.| VS | V | VS: |-VS-{1})([A-Z\s]{10,100})(Case Number)*",
                             group_index=1,
                         )
-                        .str.replace_all("Case Number:", "", literal=True)
+                        .str.replace("Case Number:", "", literal=True)
                         .str.replace(r"C$", "")
                         .str.strip()
                         .alias("Name"),
-                        pl.col("AllPagesText")
-                        .str.extract_all(
-                            r"(\d{3}\s{1}[A-Z0-9]{4}.{1,200}?.{3}-.{3}-.{3}[^a-z\n]{0,75})"
-                        )
-                        .alias("RE_Charges"),
-                        pl.col("AllPagesText")
-                        .str.extract(r"(Total:.+\$[^\n]*)")
-                        .str.replace_all(r"[^0-9|\.|\s|\$]", "")
-                        .str.extract_all(r"\s\$\d+\.\d{2}")
-                        .list.get(2)
-                        .str.replace_all(r"[^0-9\.]", "")
-                        .cast(pl.Float64, strict=False)
-                        .alias("RAWTotalBalance"),
-                        pl.col("AllPagesText")
-                        .str.extract(r"(ACTIVE[^\n]+D999[^\n]+)")
-                        .str.extract_all(r"\$\d+\.\d{2}")
-                        .list.get(-1)
-                        .str.replace(r"[\$\s]", "")
-                        .cast(pl.Float64, strict=False)
-                        .alias("RAWD999"),
-                    ]
-                )
-                all_charges = all_charges.explode("RE_Charges").select(
-                    [
-                        pl.col("Name"),
-                        pl.col("CaseNumber"),
-                        pl.col("RE_Charges")
-                        .str.replace_all(r"[A-Z][a-z][A-Za-z\s\$]+.+", "")
-                        .str.strip()
-                        .alias("Charges"),
-                        pl.when(pl.col("RAWTotalBalance").is_null())
-                        .then(pl.lit(0.0))
-                        .otherwise(pl.col("RAWTotalBalance"))
-                        .alias("TotalBalance"),
-                        pl.when(pl.col("RAWD999").is_null())
-                        .then(pl.lit(0.0))
-                        .otherwise(pl.col("RAWD999"))
-                        .alias("TotalD999"),
-                    ]
-                )
-                charges = all_charges.with_columns(
-                    [
-                        pl.col("Name"),
-                        pl.col("CaseNumber"),
-                        pl.col("Charges").str.slice(0, 3).alias("Num"),
-                        pl.col("Charges").str.slice(4, 4).alias("Code"),
-                        pl.col("Charges").str.slice(9, 1).alias("Sort"),
-                        pl.col("Charges")
-                        .str.extract(r"(\d\d?/\d\d?/\d\d\d\d)", group_index=1)
-                        .alias("CourtActionDate"),
-                        pl.col("Charges")
-                        .str.extract(
-                            r"[A-Z0-9]{3}-[A-Z0-9]{3}-[A-Z0-9]{3}\({0,1}[A-Z]{0,1}\){0,1}\.{0,1}\d{0,1}",
-                            group_index=0,
-                        )
-                        .alias("RAWCITE"),
-                        pl.col("Charges")
-                        .str.extract(
-                            r"(BOUND|GUILTY PLEA|WAIVED TO GJ|DISMISSED|TIME LAPSED|NOL PROSS|CONVICTED|INDICTED|DISMISSED|FORFEITURE|TRANSFER|REMANDED|WAIVED|ACQUITTED|WITHDRAWN|PETITION|PRETRIAL|COND\. FORF\.)",
-                            group_index=1,
-                        )
-                        .alias("CourtAction"),
-                        pl.col("Charges")
-                        .apply(
-                            lambda x: re.split(
-                                r"[A-Z0-9]{3}\s*?-[A-Z0-9]{3}\s*?-[A-Z0-9]{3}\(*?[A-Z]*?\)*?\(*?[A-Z0-9]*?\)*?\.*?\d*?",
-                                str(x),
-                            )
-                        )
-                        .alias("Split"),
-                    ]
-                )
-                charges = charges.filter(pl.col("Num").str.contains("0"))
-                charges = charges.with_columns(
-                    [
-                        pl.col("Charges")
-                        .str.contains(r"\d\d?/\d\d?/\d\d\d\d")
-                        .alias("Disposition"),
-                        pl.col("Charges").str.contains(pl.lit("FELONY")).alias("Felony"),
-                        pl.col("Charges").str.contains("GUILTY PLEA").alias("GUILTY_PLEA"),
-                        pl.col("Charges").str.contains("CONVICTED").alias("CONVICTED"),
-                    ]
+                ])
+                df = df.with_columns(
+                    pl.col("FilingCharges").apply(lambda x: re.split(r'(?m)(ALCOHOL|BOND|CONSERVATION|DOCKET|DRUG|GOVERNMENT|HEALTH|MUNICIPAL|OTHER|PERSONAL|PROPERTY|SEX|TRAFFIC)\s*$', x))
                 )
-                charges = charges.with_columns(
-                    [
-                        pl.when(pl.col("Disposition"))
-                        .then(pl.col("Split").list.get(1))
-                        .otherwise(pl.col("Split").list.get(0).str.slice(9))
-                        .str.replace(r"-   -", "", literal=True)
-                        .str.replace("1STS", "1ST", literal=True)
-                        .str.strip()
-                        .alias("RAWDESC"),
-                        pl.when(pl.col("Disposition"))
-                        .then(pl.col("Split").list.get(0).str.slice(19))
-                        .otherwise(pl.col("Split").list.get(1))
-                        .str.strip()
-                        .alias("SEG_2"),
-                        pl.when(pl.col("Disposition") == True)
-                        .then(False)
-                        .otherwise(True)
-                        .alias("Filing"),
-                    ]
-                )        
-                charges = charges.with_columns(
-                    [
-                        pl.col("SEG_2")
-                        .str.extract(
-                            r"(TRAFFIC MISDEMEANOR|BOND|FELONY|MISDEMEANOR|OTHER|TRAFFIC|VIOLATION)",
-                            group_index=1,
-                        )
-                        .str.replace("TRAFFIC MISDEMEANOR", "MISDEMEANOR")
-                        .alias("TypeDescription"),
-                        pl.col("SEG_2")
-                        .str.extract(
-                            r"(ALCOHOL|BOND|CONSERVATION|DOCKET|DRUG|GOVERNMENT|HEALTH|MUNICIPAL|OTHER|PERSONAL|PROPERTY|SEX|TRAFFIC)",
-                            group_index=1,
-                        )
-                        .alias("Category"),
-                        pl.col("RAWDESC")
-                        .str.contains(r"(A ATT|ATTEMPT|S SOLICIT|CONSP|SOLICITATION|COMPLICITY|CONSPIRACY|SOLICIT[^I]*[^O]*[^N]*)")
-                        .is_not()
-                        .alias("A_S_C_DISQ"),
-                        pl.col("Code")
-                        .str.contains(
-                            r"(OSUA|EGUA|MAN1|MAN2|MANS|ASS1|ASS2|KID1|KID2|HUT1|HUT2|BUR1|BUR2|TOP1|TOP2|TP2D|TP2G|TPCS|TPCD|TPC1|TET2|TOD2|ROB1|ROB2|ROB3|FOR1|FOR2|FR2D|MIOB|TRAK|TRAG|VDRU|VDRY|TRAO|TRFT|TRMA|TROP|CHAB|WABC|ACHA|ACAL)"
-                        )
-                        .alias("CERV_DISQ_MATCH"),
-                        pl.col("Code")
-                        .str.contains(
-                            r"(RAP1|RAP2|SOD1|SOD2|STSA|SXA1|SXA2|ECHI|SX12|CSSC|FTCS|MURD|MRDI|MURR|FMUR|PMIO|POBM|MIPR|POMA|INCE)"
-                        )
-                        .alias("PARDON_DISQ_MATCH"),
-                        pl.col("Charges")
-                        .str.contains(r"(CM\d\d|CMUR|CAPITAL)")
-                        .alias("PERM_DISQ_MATCH"),
-                    ]
+                df = df.with_columns([
+                    pl.col("FilingCharges").apply(lambda x: x[0::2][0:-1]).alias("Charge"),
+                    pl.col("FilingCharges").apply(lambda x: x[1::2]).alias("Category")
+                ])
+                df = df.explode("Charge", "Category")
+                df = df.with_columns(pl.col("Charge").str.replace_all("\n","").str.strip())
+                df = df.with_columns([
+                    pl.col("Charge").str.extract(r'(\d+)').alias("#"),
+                    pl.col("Charge").str.extract(r'\d+ ([A-Z0-9]+)').alias("Code"),
+                    pl.col("Charge").str.extract(r'\d+ [A-Z0-9]+ (.+?) [A-Z0-9]{3}-[A-Z0-9]{3}- *[A-Z0-9]{1,3}').str.replace(r'([\s-]+)$','').str.strip().alias("Description"),
+                    pl.col("Charge").str.extract(r'([A-Z0-9]{3}-[A-Z0-9]{3}- *[A-Z0-9]{1,3}\.?\d*\(?[A-Z0-9]*\)?\(?[A-Z0-9]*\)?)').str.replace(" ", "").alias("Cite"),
+                    pl.col("Charge").str.extract(r'(TRAFFIC MISDEMEANOR|BOND|FELONY|MISDEMEANOR|OTHER|TRAFFIC|VIOLATION)$').alias("TypeDescription")
+                ])
+                df = df.drop_nulls("Charge")
+                df = df.with_columns([
+                    pl.when(pl.col("Description").is_null()).then(pl.col("Charge").str.extract(r'\d+ [A-Z0-9]+ (.+?) (TRAFFIC MISDEMEANOR|BOND|FELONY|MISDEMEANOR|OTHER|TRAFFIC|VIOLATION)$', group_index=1)).otherwise(pl.col("Description")).alias("Description")
+                ])
+                # fix RULE 32 cites and descriptions
+                df = df.with_columns([
+                    pl.when(pl.col("Description").str.contains("RULE 32")).then(pl.lit("RULE 32")).otherwise(pl.col("Cite")).alias("Cite"), 
+                    pl.when(pl.col("Description").str.contains("RULE 32")).then(pl.lit("RULE 32-FELONY")).otherwise(pl.col("Description")).alias("Description")
+                ])
+                # fix PROBATION REV cites and descriptions
+                df = df.with_columns([
+                    pl.when(pl.col("Description").str.contains("PROBATION REV")).then(pl.lit("PROBATION REV")).otherwise(pl.col("Cite")).alias("Cite"), 
+                    pl.when(pl.col("Description").str.contains("PROBATION REV")).then(pl.lit("PROBATION REV")).otherwise(pl.col("Description")).alias("Description")
+                ])
+                # fix COMMUNITY CORRECTION cites and descriptions
+                df = df.with_columns([
+                    pl.when(pl.col("Description").str.contains("COMMUNITY CORRECTION REVOC")).then(pl.lit("COMMUNITY CORRECTION REV")).otherwise(pl.col("Cite")).alias("Cite"), 
+                    pl.when(pl.col("Description").str.contains("COMMUNITY CORRECTION REVOC")).then(pl.lit("COMMUNITY CORRECTION REVOC")).otherwise(pl.col("Description")).alias("Description")
+                ])
+                # fix OTHER NON MOVING VIO cites and descriptions
+                df = df.with_columns([
+                    pl.when(pl.col("Description").str.contains("OTHER NON MOVING VIO")).then(pl.lit("OTHER NON MOVING VIO")).otherwise(pl.col("Description")).alias("Description")
+                ])
+                df = df.with_columns([
+                    pl.col("TypeDescription").str.contains("FELONY").alias("Felony"),
+                    pl.col("Description").str.contains(r"(A ATT|ATTEMPT|S SOLICIT|CONSP|SOLICITATION|COMPLICITY|CONSPIRACY|SOLICIT[^I]*[^O]*[^N]*)").alias("ASCNonDisqualifying"),
+                    pl.col("Code").str.contains(r"(OSUA|EGUA|MAN1|MAN2|MANS|ASS1|ASS2|KID1|KID2|HUT1|HUT2|BUR1|BUR2|TOP1|TOP2|TP2D|TP2G|TPCS|TPCD|TPC1|TET2|TOD2|ROB1|ROB2|ROB3|FOR1|FOR2|FR2D|MIOB|TRAK|TRAG|VDRU|VDRY|TRAO|TRFT|TRMA|TROP|CHAB|WABC|ACHA|ACAL)").alias("CERVCode"),
+                    pl.col("Code").str.contains(r"(RAP1|RAP2|SOD1|SOD2|STSA|SXA1|SXA2|ECHI|SX12|CSSC|FTCS|MURD|MRDI|MURR|FMUR|PMIO|POBM|MIPR|POMA|INCE)").alias("PardonCode"),
+                    pl.col("Code").str.contains(r"(CM\d\d|CMUR)").alias("PermanentCode")
+                ])
+                df = df.with_columns([
+                    (pl.col("CERVCode") & pl.col("ASCNonDisqualifying").is_not() & pl.col("Felony")).alias("CERVCharge"),
+                    (pl.col("PardonCode") & pl.col("ASCNonDisqualifying").is_not() & pl.col("Felony")).alias("PardonToVoteCharge"),
+                    (pl.col("PermanentCode") & pl.col("ASCNonDisqualifying").is_not() & pl.col("Felony")).alias("PermanentCharge")
+                ])
+                df = df.select("Name", "CaseNumber", "#", "Code", "Description", "Cite", "TypeDescription", "Category", "Felony", "CERVCharge", "PardonToVoteCharge", "PermanentCharge")
+                df = df.with_columns(
+                    pl.concat_str(
+                        [
+                            pl.col("CaseNumber"),
+                            pl.lit(" - "),
+                            pl.col("#"),
+                            pl.lit(" "),
+                            pl.col("Cite"),
+                            pl.lit(" "),
+                            pl.col("Description"),
+                            pl.lit(" "),
+                            pl.col("TypeDescription")
+                        ]
+                    ).alias("ChargesSummary")
                 )
-                charges = charges.with_columns(
-                    [
-                        pl.when(pl.col("A_S_C_DISQ")==None)
-                        .then(True)
-                        .otherwise(pl.col("A_S_C_DISQ"))
-                        .alias("A_S_C_DISQ")
-                    ]
+            self._filing_charges = df
+            return self._filing_charges
+
+    def disposition_charges(self):
+        if isinstance(self._disposition_charges, pl.DataFrame):
+            return self._disposition_charges
+        else:
+            if not self.is_read:
+                self.read()
+            with console.status("Parsing disposition charges..."):
+                df = self.archive.select("AllPagesText", "CaseNumber")
+                df = df.select([
+                    pl.col("CaseNumber"),
+                    pl.col("AllPagesText").str.extract(r'(?s)Disposition Charges (.+?) (Sentences|Enforcement)').str.replace(r"# Code Court Action Category Cite Court Action Date\s*\n\s*", "").str.replace(r"Type Description Description Class ID\s*\n\s*", "").str.replace_all(r'(..Alacourt\.com \d\d?/\d\d?/\d\d\d\d \d)','').str.replace(r"^\s*\n\s*","").str.replace(r'\s*\n$','').alias("DispositionCharges"),
+                    pl.col("AllPagesText").str.extract(r"(Total:.+\$[^\n]*)").str.replace_all(r"[^0-9|\.|\s|\$]", "").str.extract_all(r"\s\$\d+\.\d{2}").list.get(2).str.replace_all(r"[^0-9\.]", "").cast(pl.Float64, strict=False).alias("TotalBalance"),
+                pl.col("AllPagesText").str.extract(r"(ACTIVE[^\n]+D999[^\n]+)").str.extract_all(r"\$\d+\.\d{2}").list.get(-1).str.replace(r"[\$\s]", "").cast(pl.Float64, strict=False).alias("D999"),
+                pl.col("AllPagesText")
+                .str.extract(
+                    r"(?:VS\.|V\.| VS | V | VS: |-VS-{1})([A-Z\s]{10,100})(Case Number)*",
+                    group_index=1,
+                )
+                .str.replace("Case Number:", "", literal=True)
+                .str.replace(r"C$", "")
+                .str.strip()
+                .alias("Name")
+                ])
+                df = df.with_columns(
+                    pl.col("DispositionCharges").apply(lambda x: re.split(r'(?m)^\s*(\d{3}) ', x))
                 )
-                charges = charges.filter(pl.col("TypeDescription").str.contains(r"[A-Za-z]"))
-                charges = charges.with_columns(
-                    [
-                        pl.when(pl.col("GUILTY_PLEA") | pl.col("CONVICTED"))
-                        .then(True)
-                        .otherwise(False)
-                        .alias("Conviction")
-                    ]
+                df = df.select(
+                    pl.col("Name"),
+                    pl.col("CaseNumber"),
+                    pl.col("DispositionCharges").apply(lambda x: x[0::2][1:]).alias("Row"),
+                    pl.col("DispositionCharges").apply(lambda x: x[1::2]).alias("#"),
+                    pl.col("TotalBalance"),
+                    pl.col("D999")
                 )
-                charges = charges.with_columns(
-                    [
-                        pl.when(
-                            pl.col("CERV_DISQ_MATCH")
-                            & pl.col("Felony")
-                            & pl.col("Conviction")
-                            & pl.col("A_S_C_DISQ")
-                        )
-                        .then(True)
-                        .otherwise(False)
-                        .alias("CERVDisqConviction"),
-                        pl.when(pl.col("CERV_DISQ_MATCH") & pl.col("Felony") & pl.col("A_S_C_DISQ"))
-                        .then(True)
-                        .otherwise(False)
-                        .alias("CERVDisqCharge"),
-                        pl.when(
-                            pl.col("PARDON_DISQ_MATCH")
-                            & pl.col("A_S_C_DISQ")
-                            & pl.col("Conviction")
-                            & pl.col("Felony")
-                        )
-                        .then(True)
-                        .otherwise(False)
-                        .alias("PardonDisqConviction"),
-                        pl.when(
-                            pl.col("PARDON_DISQ_MATCH") & pl.col("Felony") & pl.col("A_S_C_DISQ")
-                        )
-                        .then(True)
-                        .otherwise(False)
-                        .alias("PardonDisqCharge"),
-                        pl.when(
-                            pl.col("PERM_DISQ_MATCH")
-                            & pl.col("A_S_C_DISQ")
-                            & pl.col("Felony")
-                            & pl.col("Conviction")
-                        )
-                        .then(True)
-                        .otherwise(False)
-                        .alias("PermanentDisqConviction"),
-                        pl.when(pl.col("PERM_DISQ_MATCH") & pl.col("Felony") & pl.col("A_S_C_DISQ"))
-                        .then(True)
-                        .otherwise(False)
-                        .alias("PermanentDisqCharge"),
-                        pl.concat_str([pl.col("CaseNumber"), pl.lit("-"), pl.col("Num")]).alias(
-                            "CASENONUM"
-                        ),
-                    ]
+                df = df.explode("Row", "#")
+                df = df.with_columns(
+                    pl.col("Row").str.replace_all("\n"," ").str.strip()
                 )
-                charges = charges.with_columns(
-                    [
-                        pl.col("TotalBalance"),
-                        pl.when(
-                            pl.col("CERVDisqConviction")
-                            | pl.col("PardonDisqConviction")
-                            | pl.col("PermanentDisqConviction")
-                        )
-                        .then((pl.col("TotalBalance") - pl.col("TotalD999")))
-                        .otherwise(None)
-                        .alias("PaymentToRestore"),
-                        pl.col("RAWDESC").alias("Description"),
-                        pl.col("RAWCITE").alias("Cite")
-                    ]
+                df = df.with_columns([
+                    pl.col("Row").str.extract(r'([A-Z0-9]+)').alias("Code"),
+                    pl.col("Row").str.extract(r'(\d\d?/\d\d?/\d\d\d\d)').alias("CourtActionDate").str.to_date('%m/%d/%Y', strict=False),
+                    pl.col("Row").str.extract(r'(BOUND|GUILTY PLEA|WAIVED TO GJ|DISMISSED|TIME LAPSED|NOL PROSS|CONVICTED|INDICTED PRIOR TO ADJUDICATIO N|DISMISSED|FORFEITURE|TRANSFER|REMANDED|WAIVED|ACQUITTED|WITHDRAWN|PETITION DENIED|PRETRIAL|COND\. FORF\. SET ASIDE|COND\. FORF\.|PROBATION REVOKED|OTHER|PROBATION NT REVOKE|PROBATION/S|NO PROBABLE CAUSE|PETITION GRANTED|PROBATION TERMINATED)').str.replace("PROBATION/S","PROBATION/SANCTION").str.replace("ADJUDICATIO N", "ADJUDICATION").alias("CourtAction"),
+                    pl.col("Row").str.extract(r'([A-Z0-9]{3}-[A-Z0-9]{3}- *[A-Z0-9]{1,3}\.?\d*\(?[A-Z0-9]*\)?\(?[A-Z0-9]*\)?\(?[A-Z0-9]*\)?\d?/?\d?)').str.replace(" ","").alias("Cite"),
+                    pl.col("Row").str.extract(r'([A-Z0-9]{3}-[A-Z0-9]{3}- *[A-Z0-9]{1,3}\.?\d*\(?[A-Z0-9]*\)?&?\(?[A-Z0-9]*\)?\(?[A-Z0-9]*\)?\d?/?\d?) (.+)', group_index=2).str.strip().alias("Description"),
+                    pl.col("Row").str.extract(r'(ALCOHOL|BOND FORFEITURE|CONSERVATION|DOCKET|DRUG|GOVERNMENT PUBLIC|HEALTH|MUNICIPAL|OTHER|PERSONAL|PROPERTY|SEX OFFENSE|TRAFFIC)\s*(TRAFFIC MISDEMEANOR|BOND|FELONY|MISDEMEANOR|OTHER|VIOLATION|TRAFFIC)', group_index=2).alias("TypeDescription"),
+                    pl.col("Row").str.extract(r'(ALCOHOL|BOND FORFEITURE|CONSERVATION|DOCKET|DRUG|GOVERNMENT PUBLIC|HEALTH|MUNICIPAL|OTHER|PERSONAL|PROPERTY|SEX OFFENSE|TRAFFIC)').alias("Category")
+                ])
+                df = df.with_columns(
+                    pl.when(pl.col("TypeDescription").is_null()).then(pl.col("Row").str.extract(r'(TRAFFIC MISDEMEANOR|BOND|FELONY|MISDEMEANOR|OTHER|VIOLATION|TRAFFIC)')).otherwise(pl.col("TypeDescription")).alias("TypeDescription")
                 )
-                charges = charges.fill_null("")
-                fillers = pl.DataFrame({
-                    'Code': ['PFI3', 'NWNI', 'VDR1', 'UPCS', 'FRCC', 'T003', 'PMIO', 'UPCC', 'BEMV', 'HARA', 'TET3', 'T042', 'T707', 'SX12', 'TRAK', 'FCDC', 'TOD3', 'UAUV', 'T012', 'FR3D', 'HCOM', 'TP3D', 'VPCC', 'FORF', 'CECE', 'UDCS', 'PRO2', 'MCS1', 'ACHA', 'CECD', 'T627', 'FTCS', 'MCS2', 'PRO3', 'UAUM', 'T527', 'BRA3', 'FMUR', 'MURR', 'FPCC', 'PREC', 'STSA', 'T582', 'CM02', 'VDR4', 'VAPP', 'MAN1', 'VDR1', 'T755', 'TRAO', 'FORM', 'SVIA', 'TRAG', 'DSF1', 'MISC', 'BRA1', 'CEM1', 'CM04', 'IPCD', 'T005', 'T525', 'CM15', 'DUIF', 'T169', 'DUIM', 'T718', 'DVHF', 'TROP', 'CM10', 'CM17', 'CM01', 'VDRU', 'T770', 'ACAL', 'VDRY', 'TRFT', 'FNLE', 'RS3D', 'T806', 'TOS3', 'TSIB', 'T011', 'VAPD', 'T128', 'BHER', 'APPL', 'MRDI', 'UAUY', 'T019', 'T006', 'MAN2', 'CM18', 'NUSE', 'FBAP', 'VDRO', 'CM16', 'EDCO', 'T096', 'THBV', 'ASTM', 'SAVI', 'DVFC', 'T128', 'T071', 'CM07', 'TRBF', 'T813', 'CM03', 'TRMA', 'T783', 'T091', 'T072', 'TOS2', 'DV36', 'DSF2', 'CM08', 'DOG1', 'CEM3', 'PACS', 'T097', 'VDR2', 'BRA2', 'DVFC', 'TS3D', 'CODL', 'HAR2', 'T506', 'HGAR', 'TRCN', 'T773', 'PCUR', 'PPRE', 'T507', 'T081', 'PARA', 'MAAL', 'PCAB', 'DOG2', 'SFUF', 'OSUA', 'OSUA', 'EPH7', 'POBM', 'HWL2', 'FCPF', 'HNRL', 'DVAF', 'CPFP', 'VSMA', 'CM09', 'COMR', 'VDR5', 'TH3D', 'STG2', 'CM13', 'CNAR', 'VDR3', 'SCEF', 'CM06', 'T632', 'TRAA', 'CM13', "UUID", 'VIM2', 'TRSC', "OFFP", 'TRAY', 'COMF', 'SCR4', 'TRAT', 'TLT3', 'AGSF', 'EPH8', 'TER1', 'ECNF', 'DVE3', 'CM19', 'PSMF', 'TPCS', 'TRMF', 'CNVS', 'UPID', 'SCR6', 'COME', 'TRAQ', 'CM05', 'EAS1', 'FELO', 'CEM2', 'TS2D', 'DALE', 'CDMV', 'CM14', 'VAUA', 'COMM', 'AAPC', 'DVBF', 'TRAJ', 'DVMF', 'DV37', 'ASL1','BORK', 'T767', 'CNRR', 'PMDH', 'T043', 'LRAL', 'PUSF', 'SADV', 'TILU', 'T592', 'T513', 'FWPO', 'VPRA', 'FEED', 'T574', 'DOOM', 'CLCI', 'CODT', 'CRAB', 'STA2', 'NCOS', 'T731', 'BOCK', 'T031', 'PLUG', 'HLAG', 'CONT', 'T594', 'TREZ', 'T515', 'INSM', 'T802', 'SESS', 'HAMV', 'T505', 'TS4T', 'WOSO', 'T753', 'SIGN', 'T588', 'BLIC', 'T040', 'FIWO', 'VIM3', 'HUFV', 'TMOV', 'SETO', 'TMVV', 'LIFE', 'HWOL', 'T037', 'T622', 'T523', "PRFC", 'SHOW', 'VAUC', 'MAND', 'PCON', 'NBTR', 'UAUX', 'T799', 'TID1', 'T827', 'PDPM', 'CONS', 'SCFA', 'T116', 'T178', 'TRFM', 'TID2', 'FORT', 'T8LR', 'PAUL', 'DUIT', 'T309', 'TOWS', 'TZ67', 'APAA', 'BWNP', 'OFFM', 'UCR1', 'WAUB', 'TSTD', 'ASPC', 'APRE', 'SWOL', 'T082', 'MSTR', 'VSEX', 'MSDE', 'VAPR', 'TRWL', 'VLAT', 'OVES', 'TLEF', 'EPH5', 'AGSR', 'PLFV', 'STAA', 'T591', 'ROB1', 'TECH', 'PERT', 'PAGR', 'MCSD', 'EPHM', 'T590', 'EPHK', 'CC05', 'ELD1', 'TOFS', 'TRAZ', 'T601', 'UNLA', 'URNB', 'ESOC', 'OBUS', 'COMK', 'SOID', 'PRO1', 'UNLA'],
-                    'Description':  ['POSSESS FORGED INSTRUMENT 3RD', 'NEGOTIATING WORTHLESS INST', 'USE/POSSESS DRUG PARAPHERNALIA', 'POSS. CONTR. SUBS', 'FRAUD USE CREDIT/DEBIT CARD', 'NO DRIVERS LICENSE', 'PORN POSS MATERIAL MINORS', 'POSS CONTR SUBS INTENT DISTRIB', 'BREAK/ENTER VEHICLE', 'HARASSMENT', 'THEFT OF PROPERTY 3RD DEGREE', 'OVERWEIGHT TRUCK', 'FAIL DISPLAY INSURANCE', 'SEX ABUSE-CHILD LESS 12 YOA', 'TRAFFICKING-METHAMPHETAMINE', 'FRAUD USE CREDIT/DEBIT CARD', 'THEFT/DECEPTION 3RD', 'UNAUTHORIZED USE VEHICLE', 'FAIL STOP SIGN', 'FORGERY 3RD', 'HARASSING COMMUNICATIONS', 'THEFT OF PROPERTY 3RD DEGREE', 'POSS CONTROLLED SUBST BY FRAUD', 'BOND FORF-FELONY', 'CHEM END CHILD-EXP/CTN CTR SUB', 'UNLAW DISTRIB/FURN CONT SUBST', 'PROMOTING PROSTITUTION 2ND', 'UNLAW MANF CTN SUBS 1ST DEGREE', 'AGGRAVATED CHILD ABUSE', 'CHEM END CHILD-DEATH', 'LANE CHANGE W/O PROPER SIGNAL', 'FACILITATE TRAVEL F/ CHILD SEX', 'UNLAW MANF CTN SUBS 2ND DEGREE', 'PROMOTING PROSTITUTION 3RD', 'UNAUTHORIZED USE MOTOR VEHICLE', 'DUI-CONTROLLED SUBSTANCE', 'BURGLARY 3RD (UNOCCUPIED BLDG)', 'FELONY MURDER', 'MURDER-RECKLESS', 'ILL POSSESS CREDIT/DEBIT CARD', 'POSS/SELL PRECURSOR CHEMICALS', 'SEXUAL TORTURE/ABUSE', 'EXPIRED LICENSE', 'MURDER CAPITAL-ROBBERY', 'PARAPHERNALIA - SELL/DELIVER', 'POSSESS MARIHUANA 1ST DEGREE', 'MANSLAUGHTER-RECKLESS', 'USE/POSSESS DRUG PARAPHERNALIA', 'NO/IMP TAG LIGHT', 'TRAFFICKING-HEROIN', 'BOND FORF-MISD', 'SALVIA MISDEMEANOR POSSESSION', 'TRAFFICKING-SYNTHETIC DRUGS', 'DISCHARGE GUN OCC BLDG/VEHICLE', 'MISCELLANEOUS FILING', 'BURGLARY 3RD - DWELLING', 'CHEMICAL ENDANGER MINOR', 'MURDER CAPITAL-BURGLARY', 'ILL POSSESS CREDIT/DEBIT CARD', 'UNDER INFLUENCE CONT. SUBSTANC', 'DUI: ANY SUB WHICH IMPAIRS', 'MURDER CAPITAL-UNDER 14 YEARS', 'DUI - FELONY', 'SPEED/ 70+ MPH OR 65+ MPH', 'DUI - MISD', 'DUI: UNDER INFLU ALCOHOL', 'FELONY DV 3RD HARRASSMENT', 'TRAFFICKING-OPIUM', 'MURDER CAPITAL-TWO OR MORE PER', 'MURDER CAPITAL-VEH FR OUTSIDE', 'MURDER CAPITAL-KIDNAP', 'TRAFFICKING-MORPHINE', 'INOPERABLE BRAKE LIGHTS', 'AGGRAVATED CHILD ABUSE < SIX', 'TRAFFICKING-COCAINE', 'TRAFFICKING FENTANYL', 'GIVING FALSE NAME TO OFF', 'REC STOLEN PROP 3RD', 'NO DRIVERS LICENSE', 'THEFT OF SERVICES 3RD', 'TRAFFICKING STOLEN IDENTITIES', 'DRIVING WRONG SIDE HWY', 'POSSESS MARIHUANA 1ST DEGREE', 'NO TAG REGIS IN VEHICLE', 'BOND HEARING', 'CASE APPEALED ON', 'MURDER - INTENTIONAL', 'UNAUTHORIZED USE VEHICLE', 'FAILURE TO DIM LIGHTS', 'FAIL YIELD ROW', 'MANSLAUGHTER-INTENT, PASSION', 'MURDER CAPITAL-FIRED FROM VEHI', 'NO USER PERMIT', 'FRAUD BY AUTHORIZED PERSONS', 'DRUG PARAPHERNALIA TO MINOR', 'MURDER CAPITAL-DWELL FR OUTSID', 'ENDG WELFARE CHILD-OCCUPATION', 'MOVING TRAFFIC VIO', 'HOMICIDE BY VEHICLE', 'ALCOHOL-SALE/PERMIT UNDER AGE', 'SALVIA FELONY POSSESSION', 'FELONY DV CRIM MISCHIEF 2D/3D', 'NO TAG REGIS IN VEHICLE', 'COMBINED INFLUENCE', 'MURDER CAPITAL-FOR HIRE', 'TR-FORT.', 'MOVE OVER LAW', 'MURDER CAPITAL-RAPE/SODOMY', 'TRAFFICKING-MARIJUANA', 'IMPEDING FLOW TRAFFIC', 'DUI', 'UNDER INFLU - ANY SUBSTANCE', 'THEFT OF SERVICES 2ND', 'FELONY DV CRIM MISCHIEF 2ND', 'DISCHARGE GUN UNOCC BLDG/VEH', 'MURDER CAPITAL-SEXUAL ABUSE', 'DOG/CAT CRUELTY 1ST DEGREE', 'CHEMICAL ENDANGER MINOR/DEATH', 'PROHIBITED ACTS-MAIN BLD/DWL', 'OTHER NON MOVING VIO', 'DEL/SALE DRUG PARAPHERNALIA', 'BURGLARY 3RD - OCCUPIED BLDG', 'FELONY DV CRIM MISCHIEF 2D/3D', 'THEFT OF SERVICES 3RD DEGREE', 'CONTRIBUTING TO THE DELINQUENC', 'HARASSMENT - THREAT', 'FAIL TO YIELD EMER VEHICLE', 'FAILURE TO COMPLY - GARBAGE', 'TR-CONTEMPT', 'IMP TAIL LIGHTS-TRAILER', 'FAIL CPLY REPORTS-PRECUR CHEMS', 'POSS OF PRE-CURSOR CHEMICALS', 'FAIL TO YIELD RIGHT OF WAY', 'NO HDLGTS WHEN REQUIRED', 'FAILURE COMPLY PARK CONDITIONS', 'ALCOHOL- MINOR/POSS/CONSUME', 'POSS/CONT ALCOHOL-STATE PARK', 'DOG/CAT CRUELTY 2ND DEGREE', 'SETTING FIRE-UNCL FOREST/WOOD', 'OMMISSION/MISREP SALE SECURITI', 'OMMISSION/MISREP SALE SECURITI', 'ILL PURCHASE EPHEDRINE-INDIVID', 'PORN INTENT TO DISSEMINATE', 'HUNT-W/O NONRESIDENT LICENSE', 'FIREARM-PERSONS FORBIDDEN/POSS', 'HUNT-LEND RESIDENT LICENSE', 'FELONY DV 3RD ASSAULT 3RD', 'PISTOL-CERTAIN PERSONS FORBIDD', 'UNLAWFUL DISTRIB MARIHUANA', 'MURDER CAPITAL-ARSON', 'COMM NOTIF ACT-SCHOOL/CHILD CR', 'MANUFACTURE PARAPHERN/FIREARM', 'THEFT BY DECEPTION 3RD', 'AGGRAVATED STALKING 2ND DEGREE', 'MURDER CAPITAL-20YR PRIOR CON', 'COMM NOTIFICATION-DECLARATION', 'DEL/SALE DRUG PARAPHERNALIA', 'SCHOOL EMPLOYEE SEXUAL CONTACT', 'MURDER CAPITAL-LIFE SENTENCE', 'DUI FELONY', 'TRAFF/CONTR SUBSTANCE', 'MURDER CAPITAL-20YR PRIOR CON', "UNAUTH USE ID #", 'IMITATION DRUG DIST TO MONOR', 'SCRAP METAL/FALSIFY STATEMENT',"USE POSITION-PERSONAL GAIN", 'TRAFFICKING-HYDROMORPHONE','COMM NOTIF ACT-VICTIM/VIC FAMI', 'ILLEGAL DISPOSAL/ SCRAP TIRES', 'TRAFFICKING-3,4 METHYL AMPHETA','THEFT OF LOST PROPERTY 3RD', 'AGGRAVATED SURVEILLANCE FELONY', 'ILL PURCHASE EPHEDRINE-INDIVID', 'TERRORISM', 'ERROR CORAM NOBIS - FELONY', 'FELONY DV 3RD ONE PRIOR FELONY','CAPITAL MURDER - PROTECT ORDER', 'OBSCENE MATERIAL- DIST/POSS', 'THEFT 2ND CONTROLLED SUBSTANCE', 'TRAFF CANNABIS-W/POSS FIREARM', 'COMM NOTIF-10 DAY VERIF SUBMIT', 'POSS CONTR SUBS INTENT DISTRIB', 'SCRAP METAL/FALSE INFO', 'COM NOTIF ACT-NONRESIDENT', 'TRAFFICKING-LSD', 'MURDER CAPITAL-LAW OFF/GUARD', 'EXPLOITATION OF ASSETS 1ST', 'FELONY CASE', 'CHEMICAL ENDANGER INJURY', 'THEFT OF SERVICES 2ND DEGREE', 'DISARMING LAW ENFORCEMENT', 'UNAUTH USE MTR VEH - BY FORCE', 'MURDER CAPITAL-WITNESS', 'UNEMPLOYMENT COMP-CLASS B FEL', 'COMM NOTIF ACT-MINOR RESIDENCE', 'AIDS/ABETS PERSON COMMIT OFFEN', 'FELONY DV 3RD HARRASS COMMUNIC', 'TRAFFICKING-AMPHETAMINE', 'FELONY DV 3RD MENACING', 'FELONY DV CRIM MISCHIEF 3RD', 'ASSAULT 1ST DEGREE (DUI/BUI)','BOAT-RECKLESS OPER VESSEL', 'IMPROPER LOAD-UNSECURED', 'COMM NOTIF RESIDENCE REQ', 'HUNT/FEED AREA', 'OVERWIDE TRUCK', 'PERMITTING LIVESTOCK TO RUN AT', 'POSSESSING UNDERSIZE FISH', 'BOAT-VESS W/O SAFETY DEV/LGHT', 'IMPROPER LOAD', 'ALCOHOL-CONSUM/COMM VEH', 'DRIVE THRU BARRICADE', 'FISHING W/O PERMISSION OWNER', 'VIO. PARENTAL RESPONSIBILTY AC', 'HUNT-AREA FEEDING TAKEN PLACE', 'SPILLING LOAD ON ROAD', 'DISSEMINATE OBSCENE MATERIAL', 'CHANGING LIC PLATE-CONCEAL ID', 'CONT TO TRUANCY', 'POSS UNDERSIZED BLUE CRABS', 'STALKING  2ND DEGREE', 'NO CUT OFF SWITCH LANYARD', 'HITCHHIKING', 'BOAT-CARELESS OPER VESSEL', 'ONEWAY STREET', 'ILLEGAL ARMS - TURKEY HUNTING', 'HUNT W/O LICENSE (ALL GAME)', 'CONTEMPT OF COURT', 'BOATING UNDER THE INFLUENCE', 'FAIL/YIELD EMERG VEHICLE', 'OVERSIZED LOAD LIMIT', 'OPER VEH W/O INSURANCE', 'CAUSE/ALLOW LITTER-ROADWAY', 'SOLICIT SEX ACT WITH STUDENT', 'HUNT-BY AID MOTORIZED VESSEL', 'BLUE LIGHT LAW', 'THEFT OF SERVICES 4TH DEGREE', 'NO/ATTACHED SHUT-OFF SWITCH', 'IMP LIGHT COLORING', 'BOAT-VIO. RESTRICTIVE SIGN', 'STOPPING ON HIGHWAY', 'BOATING W/O LICENSE/CERTIF', 'OVERHEIGHT TRUCK', 'FISH-WO PERMISSION', 'IMITATION DRUG POSSESSION', 'HUNT-FROM VEHICLE', 'MOVE OVER/EMERGENCY VEHICLE', 'DIST OBSCENE MATERIAL/SCHOOL', 'MOVE OVER LAW VIOLATIONS', 'BOAT-VESSEL W/O LIFE PRE.', 'HUNT-W/O LICENSE', 'MOTORCYCLE NO-HELMET', 'NO TAG - UTILITY TRAILER', 'DUI 0.08 BAC OR ABOVE', 'PT-RL F/CN', 'SHOW CAUSE DKT/HEARING', 'UNEMPLOYMENT COMP-VIOLATION', 'WIRT OF MANDAMUS', 'PISTOL-CERTAIN PERSONS FORBIDD', 'NO ANT BUCK/TURKEY HAR RECORD', 'UNAUTHORIZED USE VEHICLE', 'PEDESTRIAN-SOL EMPLY/BUSN/CONT', 'IGNITION INTERLOCK MISDEMEANOR', 'FAIL UPDATE DL NAME/ADDRESS', 'DISTRIB HARMFUL MATERIAL-MINOR', 'CONSERVATION', 'SCIRE FACI', 'CMV W/O PROPER DOCUMENTS', 'DUI .08 OR MORE', 'TRAFFIC/MISC', 'IGNITION INTERLOCK VIOLATIONS', 'FORFEITURE-TRAFFIC', 'CAUSE/ALLOW LITTER ON ROADWAY', 'ALCOHOL-POSS UNTAXED LIQ', 'DUI TRIAL DOCKET', 'FAIL TO STOP AS REQUIRED', 'BOAT-SKING W/O MIRROR\\OBSERVER', 'CZ SLOWING/STOP W/O PROPER SIG', 'ALCOHOL - ON PUBLIC ACCESS AREA', 'BURN W/OUT NECESSARY PRECAUTIO', 'USE OFF POSITION- PERSONAL GAIN', 'UNIFIED CARRIER REGISTRATION', 'WHLSE SALE ALCOHOL UNA BUYER', 'KNOWINGLY TRANSMIT EXPOSE STD', 'ASPC-OTHER', 'ALCOHOL-ON OFF PREMISES LI', 'ALCOHOL-SELL W/O LICENSE', 'FAILURE TO DIM HEADLIGHTS', 'NO MASTER PLUMBER CERTIFICATE', 'VIOLATION COMMUNITY NOT ACT', 'MISDEMEANOR', 'VIOL POSTED RULE-WILDLIFE AREA', 'WASH SHRIMP TRAWL- CLOSED AREA', 'VIOLATION', 'OPER VESSEL W/O EMERG SHUTOFF', 'INTERSTATE/LEFT LANE 1.5 MILES', 'SINGLE SALE-EPHEDRINE PRODUCT', 'AGGRAVATED SURVEILLANCE MISD', 'HUNT-POSS LOAD GUN IN VEH', 'STALKING AGGRAVATED 1ST DEGREE', 'HANDICAPPED PARKING VIOLATION', 'ROBBERY 1ST', 'TECH VIOL PROBATION', 'UNLAW SALE TOBACCO W/O PERMIT', 'ALCOHOL-POSS MORE THAN 5 GAL.', 'WRONG1MANF CTN SUBS 1ST DEGREE', 'DRUG OFFENDER EPHEDRINE MISD', 'FAIL TO STOP EXIT PARKING LOT', 'SALE EPHEDRINE 2ND CONVICTION', 'CRIM CONSPIRACY -FELONY A', 'ELDER ABUSE AND NEGLECT 1ST', 'FALSE STATEMENT/EXPIRED TAG', 'FAILURE TO PARTICIPATE IN GARG', 'CROSS MEDIAN/IMP USE DIV HGWY', 'UNLAWFUL ASSEMBLY', 'ILLEGAL USE OF SYNTHETIC URINE', 'ELECTRONIC SOLICITION OF CHILD', 'SHOOT/DISC FIREARM OCC BUS/BLD', 'VIOL COM NOTIF ACT/EMPLOYMENT', 'SEX OFFENDER MANDATORY ID', 'PROMOTING PROSTITUTION 1ST', 'UNLAWFUL ASSEMBLY'],
-                    'Cite': ['13A-009-006.1', '13A-009-013.1', '13A-012-260(C)', '13A-012-212(A)', '13A-012-212(A)', '032-006-001(A)', '13A-012-192(B)', '013-012-192(B)', '13A-008-011(B)', '13A-011-008(A)', '13A-008-004.1', '032-009-020(4)', '032-07A-016(B)', '13A-006-069.1', '13A-012-231(11)', '13A-009-014(B)', '13A-008-004.1', '13A-008-011(A)', '032-05A-112(B)', '13A-009-003.1', '13A-011-008(B)', '13A-008-4.1', '13A-012-212(A)', '- -BOND FORT', '026-015-003.2(A)', '13A-012-211', '13A-012-112', '13A-012-218', '026-015-003.1(A)', '026-015-003.2(A)', '032-05A-133', '13A-006-125', '13A-012-217', '13A-012-113', '032-008-081', '032-05A-191(A)', '13A-007-007(A)', '13A-006-002(A)', '13A-006-002(A)', '13A-009-014(A)', '020-002-190(B)', '13A-006-065.1', '032-006-001(B)', '13A-005-040(A)', '13A-012-260(D)', '13A-012-213(A)', '13A-006-003(A)', '13A-012-260(C)', '032-005-240(C)', '13A-012-231(3)', '- -BOND FORT', '13A-012-214.1', '13A-012-231(12)', '13A-011-061(B)', '', '13A-007-007(A)', '026-015-3.2(A)', '13A-005-040(A)', '13A-009-014(A)', '032-05A-191(A)', '032-05A-191(A)', '13A-005-040(A)', '032-05A-191(A)', '032-05A-171(4)', '032-05A-191(A)', '032-05A-191(A)', '13A-006-132(D)', '13A-012-231(3)', '13A-005-040(A)', '13A-005-040(A)', '13A-005-040(A)', '13A-012-231(3)', '032-005-241(B)', '025-015-03.1(B)', '13A-012-231(2)', '13A-012-231(13)', '13A-009-018.1', '13A-008-18.1', '032-006-018(A)', '13A-008-010.3', '13A-008-193(B)', '032-05A-080(A)', '13A-012-213(A)', '040-012-260(B)', '', '', '13A-006-002(A)', '13A-008-011(A)', '032-005-242(C)', '032-05A-112(C)', '13A-006-003(A)', '13A-005-040(A)', '033-015-007(C)', '13A-009-014.1', '13A-012-260(E)', '13A-005-040(A)', '13A-013-006(A)', '', '032-05A-190.1', '028-03A-025(A)', '13A-012-214.1', '13A-006-132(D)', '040-012-260(B)', '032-05A-191(A)', '13A-005-040(A)', '', '032-05A-058.2', '13A-005-040(A)', '13A-012-231(1)', '032-05A-080(B)', '032-05A-191(A)', '032-05A-191(A)', '13A-008-010.2', '13A-006-132(D)', '13A-011-061(C)', '13A-005-040(A)', '13A-011-241(A)', '026-015-3.2(A)', '020-002-071(A)', '', '13A-012-260(E)', '13A-007-007(A)', '13A-006-132(D)', '13A-008-010.25', '012-015-111(A)', '13A-011-008(A)', '032-05A-115(A)', '022-027-003(A)', '', '032-005-240(C)', '020-002-190(A)', '020-002-181(D)', '032-05A-082(2)', '032-005-240(A)', '220-005-013(2)', '028-03A-025(A)', '220-005-016(4)', '13A-011-241(B)', '009-013-011(B)', '008-006-017(A)', '008-006-017(A)', '020-002-190(C)', '13A-012-192(A)', '009-011-051(C)', '13A-011-072(A)', '009-011-051(B)', '13A-006-132(D)', '13A-011-072(A)', '13A-012-211(A)', '13A-005-040(A)', '015-020-026(A)', '13A-012-260(D)', '13A-008-04.1', '13A-006-091.1', '13A-005-040(A)', '015-020-022(A)', '13A-012-260(E)', '13A-006-082(A)', '13A-005-040(A)', '032-05A-191(A)', '13A-012-231(12)', '13A-005-040(A)', "032-008-086(D)", '020-008-086(D)', '032-008-087(S)(2)', '036-025-005(A)','13A-012-231(5)', '015-020-026(B)', '022-40A-19(A)(4)', '13A-012-231(6)', '13A-008-008.1', '13A-011-32.1', '020-002-190(C)(4)', '13A-010-152(A)', '', '13A-006-132(E)', '13A-005-040(19)', '13A-012-200.2(1)', '13A-008-004(D)', '13A-012-231(13)', '015-020-024(B)', '13A-012-211(C)', '13A-008-031(D)', '015-020-25.1', '13A-012-231(9)', '13A-005-040(A)(5)', '038-009-007(G)', '', '026-015-3.2(A)(2)', '13A-008-010.2', '13A-010-005.1', '13A-008-011(A)(4)', '13A-005-040(A)(14)', '025-004-145(A)(1)A', '015-020-026(C)', '13A-002-023(2)', '13A-006-132(D)', '13A-012-231(10)', '13A-006-132(D)', '13A-006-132(D)', '13A-006-020(A)(5)','033-005-070(A)', '032-005-076(B)', '015-020-021(C)', '220-002-011(8', '032-009-020(1', '003-005-002(D)', '220-003-030(2', '033-005-022(A)', '032-005-076(B)', '032-006-049.1', '023-005-002(B)', '220-002-044(6', '016-028-012(A)', '220-002-011(8', '032-005-076(A)', '13A-012-200.3', '032-008-086(E)', '012-015-013(A)', '220-003-031(1', '13A-006-090.1', '033-005-051(C)', '032-05A-216(A)', '033-005-070(B)', '032-05A-087(B)', '220-002-002(3', '009-011-051(A)', '012-011-030', '032-05A-191.3', '032-05A-115(A)', '032-009-029(A)', '032-07A-016(1', '032-005-076(C)', '13A-006-082(B)', '220-002-011(1', '032-05A-115(C)', '13A-008-010.3', '033-005-072(A)', '032-005-242(G)', '220-006-019(4', '032-05A-136(A)', '033-005-052(A)', '032-009-020(2', '009-011-091(A)', '020-002-143(C)', '220-002-011(1', '032-05A-058.2', '13A-006-082.1', '032-05A-058.2', '220-006-011(1', '009-011-051(A)', '032-05A-245(A)', '040-012-252(A)', '032-05A-191(A)1','','','025-004-145(A)(1)C','','13A-011-072(B)', '220-002-146(2)', '13A-008-011(A)2', '032-05A-216(B)', '032-05A-191.4(J)', '760-X-1-07(7)', '13A-012-200.5(1)', '', '', '', '032-05A-191(A)1', '', '032-05A-191.4(L)','- -BOND FORT', '032-005-076(C)(1)', '028-04-020', '','','033-005-026(A)', '032-05A-133(C)', '220-002-037(13)', '009-013-011(B)(2)', '036-025-005(A)', 'PSC-3.2-016', '028-03A-025(A)(2)', '022-11A-021(C)', '', '028-03A-025(A)(4)', '028-03A-025(A)(14)', '032-005-242(C)(2)', '034-037-001(8)', '', '', '220-002-055(1)(BB)', '220-003-001(5)', '', '033-005-072(B)', '032-05A-080(D)(1)', '020-002-190(C)(2)', '13A-011-32.1', '220-002-055(1)(K)', '13A-006-091', '032-006-233.1', '13A-008-041', '015-022-054.1', '028-011-008', '028-004-115', '13A-012-218', '020-002-190.2(K)', '032-05A-153', '020-002-190.2(K)', '13A-006-192', '032-006-219', '022-027-007', '032-05A-090', '13A-011-005', '13A-012-340', '13A-006-122', '13A-004-003', '13A-011-061.1', '015-020-023.1', '015-020-026.2', '13A-012-111', '13A-011-005'] 
-                    }
+                # fix RULE 32 cites and descriptions
+                df = df.with_columns([
+                    pl.when(pl.col("Row").str.contains("RULE 32")).then(pl.lit("RULE 32")).otherwise(pl.col("Cite")).alias("Cite"), 
+                    pl.when(pl.col("Row").str.contains("RULE 32")).then(pl.lit("RULE 32-FELONY")).otherwise(pl.col("Description")).alias("Description")
+                ])
+                # fix PROBATION REV cites and descriptions
+                df = df.with_columns([
+                    pl.when(pl.col("Row").str.contains("PROBATION REV")).then(pl.lit("PROBATION REV")).otherwise(pl.col("Cite")).alias("Cite"), 
+                    pl.when(pl.col("Row").str.contains("PROBATION REV")).then(pl.lit("PROBATION REV")).otherwise(pl.col("Description")).alias("Description")
+                ])
+                # fix COMMUNITY CORRECTION cites and descriptions
+                df = df.with_columns([
+                    pl.when(pl.col("Row").str.contains("COMMUNITY CORRECTION REVOC")).then(pl.lit("COMMUNITY CORRECTION REV")).otherwise(pl.col("Cite")).alias("Cite"), 
+                    pl.when(pl.col("Row").str.contains("COMMUNITY CORRECTION REVOC")).then(pl.lit("COMMUNITY CORRECTION REVOC")).otherwise(pl.col("Description")).alias("Description")
+                ])
+                # fix OTHER NON MOVING VIO descriptions
+                df = df.with_columns([
+                    pl.when(pl.col("Row").str.contains("OTHER NON MOVING VIO")).then(pl.lit("OTHER NON MOVING VIO")).otherwise(pl.col("Description")).alias("Description")
+                ])
+                # fix BOND FORFEITURE cites and descriptions
+                df = df.with_columns([
+                    pl.when(pl.col("Row").str.contains("BOND FORFEITURE")).then(pl.lit("BOND FORT")).otherwise(pl.col("Cite")).alias("Cite"), 
+                    pl.when(pl.col("Row").str.contains("BOND FORFEITURE")).then(pl.lit("BOND FORF-FELONY")).otherwise(pl.col("Description")).alias("Description")
+                ])
+                # fix - - cite descriptions
+                df = df.with_columns(
+                    pl.when(pl.col("Description").is_null()).then(pl.col("Row").str.extract(r'\s*-\s*-\s*(.+)')).otherwise(pl.col("Description")).alias("Description")
                 )
-                for r in fillers.rows():
-                    charges = charges.with_columns(
+                df = df.drop_nulls("Row")
+                ## charge sort
+                df = df.with_columns([
+                    pl.col("CourtAction").str.contains(r"GUILTY|CONVICTED").alias("Conviction"),
+                    pl.col("TypeDescription").str.contains("FELONY").alias("Felony"),
+                    pl.col("Description").str.contains("(A ATT|ATTEMPT|S SOLICIT|CONSP|SOLICITATION|COMPLICITY|CONSPIRACY|SOLICIT[^I]*[^O]*[^N]*)").alias("ASCNonDisqualifying"),
+                    pl.col("Code").str.contains(r"(OSUA|EGUA|MAN1|MAN2|MANS|ASS1|ASS2|KID1|KID2|HUT1|HUT2|BUR1|BUR2|TOP1|TOP2|TP2D|TP2G|TPCS|TPCD|TPC1|TET2|TOD2|ROB1|ROB2|ROB3|FOR1|FOR2|FR2D|MIOB|TRAK|TRAG|VDRU|VDRY|TRAO|TRFT|TRMA|TROP|CHAB|WABC|ACHA|ACAL)").alias("CERVCode"),
+                    pl.col("Code").str.contains(r"(RAP1|RAP2|SOD1|SOD2|STSA|SXA1|SXA2|ECHI|SX12|CSSC|FTCS|MURD|MRDI|MURR|FMUR|PMIO|POBM|MIPR|POMA|INCE)").alias("PardonCode"),
+                    pl.col("Code").str.contains(r"(CM\d\d|CMUR)").alias("PermanentCode")
+                ])
+                df = df.with_columns([
+                    (pl.col("CERVCode") & pl.col("ASCNonDisqualifying").is_not() & pl.col("Felony")).alias("CERVCharge"),
+                    (pl.col("PardonCode") & pl.col("ASCNonDisqualifying").is_not() & pl.col("Felony")).alias("PardonToVoteCharge"),
+                    (pl.col("PermanentCode") & pl.col("ASCNonDisqualifying").is_not() & pl.col("Felony")).alias("PermanentCharge"),
+                    (pl.col("CERVCode") & pl.col("ASCNonDisqualifying").is_not() & pl.col("Conviction") & pl.col("Felony")).alias("CERVConviction"),
+                    (pl.col("PardonCode") & pl.col("ASCNonDisqualifying").is_not() & pl.col("Conviction") & pl.col("Felony")).alias("PardonToVoteConviction"),
+                    (pl.col("PermanentCode") & pl.col("ASCNonDisqualifying").is_not() & pl.col("Conviction") & pl.col("Felony")).alias("PermanentConviction")
+                ])
+                df = df.with_columns([
+                    pl.when(pl.col("D999").is_null()).then(pl.lit(0.0)).otherwise(pl.col("D999")).alias("D999"),
+                    pl.when(pl.col("TotalBalance").is_null()).then(pl.lit(0.0)).otherwise(pl.col("TotalBalance")).alias("TotalBalance")
+                ])
+                df = df.with_columns([
+                    pl.when(pl.col("CERVConviction") | pl.col("PardonToVoteConviction") | pl.col("PermanentConviction")).then(pl.col("TotalBalance") - pl.col("D999")).otherwise(None).alias("PaymentToRestore")
+                ])
+                df = df.select("Name", "CaseNumber", "#", "Code", "Description", "Cite", "TypeDescription", "Category", "CourtAction", "CourtActionDate", "TotalBalance", "PaymentToRestore", "Conviction", "Felony", "CERVCharge", "PardonToVoteCharge", "PermanentCharge", "CERVConviction", "PardonToVoteConviction", "PermanentConviction")
+                df = df.with_columns(
+                    pl.concat_str(
                         [
-                            pl.when(pl.col("Code")==r[0])
-                            .then(r[1])
-                            .otherwise(pl.col("Description"))
-                            .alias("Description"),
-                            pl.when(pl.col("Code")==r[0])
-                            .then(r[2])
-                            .otherwise(pl.col("Cite"))
-                            .alias("Cite")
+                            pl.col("CaseNumber"),
+                            pl.lit(" - "),
+                            pl.col("#"),
+                            pl.lit(" "),
+                            pl.col("Cite"),
+                            pl.lit(" "),
+                            pl.col("Description"),
+                            pl.lit(" "),
+                            pl.col("TypeDescription"),
+                            pl.lit(" "),
+                            pl.col("CourtAction"),
+                            pl.lit(" "),
+                            pl.col("CourtActionDate"),
                         ]
-                    )
-                charges = charges.with_columns(
-                    [
-                        pl.when((pl.col("Code")=="VIM1") & (pl.col("Description").eq("")))
-                        .then("IMITATION DRUG MANUF/DIST")
-                        .otherwise(pl.col("Description"))
-                        .alias("Description"),
-                        pl.when((pl.col("Code")=="VIM1") & (pl.col("Cite").eq("")))
-                        .then("020-002-143(A)")
-                        .otherwise(pl.col("Cite"))
-                        .alias("Cite")
-                    ]
+                    ).alias("ChargesSummary")
                 )
-                charges = charges.with_columns(
-                    [
-                        pl.col("Charges").str.extract(r'\s(A|S|C|P)\s').alias("ID"),
-                        pl.concat_str(
-                            [
-                                pl.col("CaseNumber"),
-                                pl.lit(" - "),
-                                pl.col("Num"),
-                                pl.lit(" "),
-                                pl.col("Cite"),
-                                pl.lit(" "),
-                                pl.col("Description"),
-                                pl.lit(" "),
-                                pl.col("TypeDescription"),
-                                pl.lit(" "),
-                                pl.col("CourtAction"),
-                                pl.lit(" "),
-                                pl.col("CourtActionDate"),
-                            ]
-                        )
-                        .str.strip()
-                        .str.replace(r",$", "")
-                        .str.replace_all(r"\s+", " ")
-                        .str.replace(r"\.\s\.\s", ".")
-                        .str.replace(r'\s[ASC]\s'," ")
-                        .alias("ChargesSummary")
-                    ]
-                )
-                charges = charges.with_columns(
-                    [
-                        pl.when(pl.col("Charges").str.contains("ATTEMPT").is_not() & pl.col("ID").eq("A"))
-                        .then("")
-                        .otherwise(pl.col("ID"))
-                        .alias("ID"),
-                        pl.col("Description")
-                        .str.replace(r'^\.\d?\s','')
-                        .str.replace(r'\s[ASC]\s', " ")
-                        .str.replace(r'^[ASC]\s', "")
-                    ]
-                )
-                charges = charges.with_columns(
-                    [
-                        pl.when(pl.col("ID").eq("C") & pl.col("Description").eq("ROBBERY 1ST"))
-                        .then("CONSPIRACY -ROBBERY 1ST DEGREE")
-                        .otherwise(pl.col("Description"))
-                        .alias("Description"),
-                        pl.when(pl.col("ID").eq("C") & pl.col("Description").eq("ROBBERY 1ST"))
-                        .then(False)
-                        .otherwise(pl.col("CERVDisqCharge"))
-                        .alias("CERVDisqCharge")
-                    ]
-                )
-                charges = charges.with_columns(
-                    [
-                        pl.when(pl.col("Charges").str.contains("WILFULL FAILURE TO RETURN TO P"))
-                        .then("")
-                        .otherwise(pl.col("ID"))
-                        .alias("ID")
-                    ])
-                charges = charges.fill_null('')
-                charges = charges.with_columns(
-                    [
-                        pl.col("CourtActionDate").str.to_date("%m/%d/%Y", strict=False),
-                        pl.col("Category").cast(pl.Categorical),
-                        pl.col("TypeDescription").cast(pl.Categorical),
-                        pl.col("CourtAction").cast(pl.Categorical),
-                    ]
-                )
-                charges = charges.select(
-                    "Name",
-                    "CaseNumber",
-                    "Num",
-                    "Code",
-                    "Cite",
-                    "ID",
-                    "Description",
-                    "TypeDescription",
-                    "Category",
-                    "CourtAction",
-                    "CourtActionDate",
-                    "TotalBalance",
-                    "PaymentToRestore",
-                    "Conviction",
-                    "Felony",
-                    "CERVDisqCharge",
-                    "CERVDisqConviction",
-                    "PardonDisqCharge",
-                    "PardonDisqConviction",
-                    "PermanentDisqCharge",
-                    "PermanentDisqConviction",
-                    "Filing",
-                    "Disposition",
-                    "ChargesSummary"
-                )
-            self._charges = charges
-            return self._charges
-    
+            self._disposition_charges = df
+            return self._disposition_charges
+
     def sentences(self):
         if isinstance(self._sentences, pl.DataFrame):
             return self._sentences
         else:
             if not self.is_read:
                 self.read()
             with console.status("Parsing sentences..."):
@@ -2367,118 +2246,102 @@
     def case_action_summary(self):
         if isinstance(self._case_action_summary, pl.DataFrame):
             return self._case_action_summary
         else:
             if not self.is_read:
                 self.read()
             with console.status("Parsing case action summaries..."):
-                cas = self.archive.select(
-                    [
-                        pl.col("CaseNumber"),
-                        pl.col("AllPagesText")
-                        .str.extract(r'(?s)Case Action Summary\s*\n\s*Operator\s*\n\s*(.+?)Date')
-                        .str.split("\n")
-                        .alias("CAS"),
-                    ]
+                df = self.archive.select("AllPagesText", "CaseNumber")
+                df = df.select(
+                    pl.col("CaseNumber"),
+                    pl.col("AllPagesText").str.extract(r'(?s)Case Action Summary(.+) Date').str.replace(r"\s*\n\s*Operator\s*","").alias("CAS")
+                )
+                df = df.with_columns(
+                    pl.col("CAS").apply(lambda x: re.split(r'(\d\d?/\d\d?/\d\d\d\d)\s*\n', x))
                 )
-                cas = cas.explode("CAS")
-                cas = cas.with_columns(pl.col("CAS").str.strip().str.replace(r'^(..Alacourt\.com \d\d?/\d\d?/\d\d\d\d \d)','').str.strip())
-                cas = cas.filter(pl.col("CAS").str.contains("[A-Z]"))
-                cas = cas.with_columns([
-                    pl.col("CAS").str.extract(r'(\d\d?/\d\d?/\d\d\d\d)$').str.to_date('%m/%d/%Y', strict=False).alias("Date"),
-                    pl.col("CAS").str.extract(r'(\d\d?\:\d\d [A|P]M) \d\d?/\d\d?/\d\d\d\d$').alias("Time"),
-                    pl.col("CAS").str.extract(r'([^\s]{4}) \d\d?\:\d\d [A|P]M \d\d?/\d\d?/\d\d\d\d$').alias("Code"),
-                    pl.col("CAS").str.extract(r'(.+) [^\s]{4} \d\d?\:\d\d [A|P]M \d\d?/\d\d?/\d\d\d\d$').str.replace(r'^([A-Z]{3} )','').alias("Comments"),
-                    pl.col("CAS").str.extract(r'^([A-Z]{3}) ').alias("Operator")
-                ])
-                cas = cas.select("CaseNumber", "Date", "Time", "Code", "Comments", "Operator")
-                cas = cas.filter(pl.col("Date").is_null().is_not())
-            self._case_action_summary = cas
+                df = df.select([
+                    pl.col("CaseNumber"),
+                    pl.col("CAS").apply(lambda x: x[0::2][0:-1]).alias("Row"),
+                    pl.col("CAS").apply(lambda x: x[1::2]).alias("Date")
+                ])
+                df = df.explode("Row", "Date")
+                df = df.with_columns(
+                    pl.col("Row").str.replace(r'..Alacourt\.com \d\d?/\d\d/\d\d\d\d \d+','').str.strip()
+                )
+                df = df.select([
+                    pl.col("CaseNumber"),
+                    pl.col("Date").str.to_date('%m/%d/%Y', strict=False),
+                    pl.col("Row").str.extract(r'^(\w |\w\w\w |\w\w\w\d\d\d )').str.strip().alias("Operator"),
+                    pl.col("Row").str.extract(r'(?s)^(\w |\w\w\w |\w\w\w\d\d\d )?(.+?) ([A-Z0-9-]+) (\d\d?:\d\d [AP]M)', group_index=2).str.replace("\n","").str.strip().alias("Description"),
+                    pl.col("Row").str.extract(r'(?s)^(\w |\w\w\w |\w\w\w\d\d\d )?(.+?) ([A-Z0-9-]+) (\d\d?:\d\d [AP]M)', group_index=3).alias("Code"),
+                    pl.col("Row").str.extract(r'(?s)^(\w |\w\w\w |\w\w\w\d\d\d )?(.+?) ([A-Z0-9-]+) (\d\d?:\d\d [AP]M)', group_index=4).alias("Time")
+                ])
+                df = df.filter(pl.col("Description").is_null().is_not())
+            self._case_action_summary = df
             return self._case_action_summary
     
     def financial_history(self):
         if isinstance(self._financial_history, pl.DataFrame):
             return self._financial_history
         else:
             if not self.is_read:
                 self.read()
             with console.status("Parsing financial history..."):
-                fh = self.archive.with_columns(
-                    pl.col("AllPagesText")
-                    .str.extract_all(
-                        r"(\d\d/\d\d/\d\d\d\d)\s(RECEIPT|CREDIT)\s(\$\d+\.\d\d)\s(\w\d\d\d)\s(\d\d\d)\s(\w)\s(....)\s(\d{8})\s(\d{7})\s(\w{3})"
-                    )
-                    .alias("FinancialHistory")
-                )
-                fh = fh.explode("FinancialHistory")
-                fh = fh.with_columns(
-                    [
-                        pl.col("FinancialHistory")
-                        .str.extract(r"(\d\d?/\d\d?/\d\d\d\d)")
-                        .str.to_date("%m/%d/%Y", strict=False)
-                        .alias("TransactionDate"),
-                        pl.col("FinancialHistory")
-                        .str.extract(r"(RECEIPT|CREDIT)")
-                        .alias("Description"),
-                        pl.col("FinancialHistory")
-                        .str.extract(r"(\$\d+\.\d\d)")
-                        .str.replace(r"\$", "")
-                        .str.strip()
-                        .cast(pl.Float64, strict=False)
-                        .alias("Amount"),
-                        pl.col("FinancialHistory")
-                        .str.extract(r"\s(\w\d\d\d)\s")
-                        .alias("FromParty"),
-                        pl.col("FinancialHistory").str.extract(r"\s(\d\d\d)\s").alias("ToParty"),
-                        pl.col("FinancialHistory").str.extract(r"\s(\w)\s").alias("AdminFee"),
-                        pl.col("FinancialHistory")
-                        .str.extract(r"\s([A-Z]{2}[A-Z0-9]{2})\s")
-                        .alias("DisbursementAccount"),
-                        pl.col("FinancialHistory")
-                        .str.extract(r"\s([0-9]{8})\s")
-                        .alias("ReceiptNumber"),
-                        pl.col("FinancialHistory")
-                        .str.extract(r"\s([0-9]{7})\s")
-                        .alias("TransactionBatch"),
-                        pl.col("FinancialHistory").str.extract(r"\s([A-Z]{3})$").alias("Operator"),
-                    ]
+                df = self.archive.select("CaseNumber", "AllPagesText")
+                df = df.select(
+                    pl.col("CaseNumber"),
+                    pl.col("AllPagesText").str.extract(r'(?s)Financial History(.+)Requesting Party').str.replace(r'(\s*\n\s*Description From Party To Party Admin Fee\s*)','').str.replace(r'(Money Type\s*)','').str.replace(r'(Reason Disbursement Accoun\s*)','').str.replace(r'(Transaction Batch\s*)','').str.replace(r'(Operator\s*)','').alias("FinancialHistory")
                 )
-                fh = fh.select(
-                    "CaseNumber",
-                    "TransactionDate",
-                    "Description",
-                    "DisbursementAccount",
-                    "TransactionBatch",
-                    "ReceiptNumber",
-                    "Amount",
-                    "FromParty",
-                    "ToParty",
-                    "AdminFee",
-                    "Operator",
+                df = df.with_columns(
+                    pl.col("FinancialHistory").apply(lambda x: re.split(r'(\s\w{3}\s*\n)', x))
                 )
-                fh = fh.drop_nulls()
-                fh = fh.fill_null("")
-            self._financial_history = fh
+                df = df.select([
+                    pl.col("CaseNumber"),
+                    pl.col("FinancialHistory").apply(lambda x: x[0::2][0:-1]).alias("Row"),
+                    pl.col("FinancialHistory").apply(lambda x: x[1::2]).alias("Operator")
+                ])
+                df = df.explode("Row", "Operator")
+                df = df.with_columns([
+                    pl.col("Operator").str.strip(),
+                    pl.col("Row").str.replace(r'..Alacourt\.com \d\d?/\d\d?/\d\d\d\d \d+','').str.strip(),
+                ])
+                df = df.select([
+                    pl.col("CaseNumber"),
+                    pl.col("Row").str.extract(r'^(\d\d/\d\d/\d\d\d\d)').str.to_date('%m/%d/%Y', strict=False).alias("TransactionDate"),
+                    pl.col("Row").str.extract(r'^\d\d/\d\d/\d\d\d\d (.+?)\s*\n?\s*\$').alias("Description"),
+                    pl.col("Row").str.extract(r'\$[0-9,]+\. ?\d\d [A-Z0-9]{4} *[A-Z0-9]+ ?\w *([A-Z0-9]{4})').alias("DisbursementAccount"),
+                    pl.col("Row").str.extract(r'\$[0-9,]+\. ?\d\d [A-Z0-9]{4} *[A-Z0-9]+ ?\w *[A-Z0-9]{4} *\d+ (\d+)').alias("TransactionBatch"),
+                    pl.col("Row").str.extract(r'\$[0-9,]+\. ?\d\d [A-Z0-9]{4} *[A-Z0-9]+ ?\w *[A-Z0-9]{4} *(\d+)').alias("ReceiptNumber"),
+                    pl.col("Row").str.extract(r'\$([0-9,]+\. ?\d\d)').str.replace(",","").cast(pl.Float64, strict=False).alias("Amount"),
+                    pl.col("Row").str.extract(r'\$[0-9,]+\. ?\d\d ([A-Z0-9]{4})').alias("FromParty"),
+                    pl.col("Row").str.extract(r'\$[0-9,]+\. ?\d\d [A-Z0-9]{4} *([A-Z0-9]{3,4})? ').alias("ToParty"),
+                    pl.col("Row").str.extract(r' (\w) [A-Z0-9]{4} *\d+ \d+').alias("AdminFee"),
+                    pl.col("Operator")
+                ])
+                df = df.drop_nulls("Operator")
+            self._financial_history = df
             return self._financial_history
     
     def witnesses(self):
         if isinstance(self._witnesses, pl.DataFrame):
             return self._witnesses
         else:
             if not self.is_read:
                 self.read()
             with console.status("Parsing witnesses tables..."):
                 df = self.archive
-                df = df.with_columns(
+                df = df.select(
+                    pl.col("CaseNumber"),
                     pl.col("AllPagesText").str.extract(r'(?s)SJIS Witness List\s*\n\s*Date Issued\s*\n\s*Subpoena(.+?)Date').alias("Witnesses")
                 )
                 df = df.with_columns(
                     pl.col("Witnesses").apply(lambda x: re.split(r'( [A-Z0-9]{4}\s*\n)', x))
                 )
-                df = df.with_columns([
+                df = df.select([
+                    pl.col("CaseNumber"),
                     pl.col("Witnesses").apply(lambda x: x[1::2]).alias("WitnessNo"),
                     pl.col("Witnesses").apply(lambda x: x[0::2][0:-1]).alias("Row")
                 ])
                 df = df.explode("WitnessNo","Row")
                 df = df.with_columns([
                     pl.col("WitnessNo").str.strip(),
                     pl.col("Row").str.replace("\n","").str.strip()
@@ -2535,73 +2398,49 @@
     def images(self):
         if isinstance(self._images, pl.DataFrame):
             return self._images
         else:
             if not self.is_read:
                 self.read()
             with console.status("Parsing images tables..."):
-                images = self.archive.select(
-                    [
-                        pl.col("CaseNumber"),
-                        pl.col("AllPagesText")
-                        .str.extract(
-                            r"(Images\s+?Pages)([^\\n]*)(END OF THE REPORT)", group_index=2
-                        )
-                        .str.strip()
-                        .alias("ImagesChunk"),
-                    ]
-                )
-                images = images.select(
-                    [
-                        pl.col("CaseNumber"),
-                        pl.col("ImagesChunk")
-                        .str.replace_all("© Alacourt.com", "", literal=True)
-                        .str.split("\n")
-                        .alias("Images"),
-                    ]
+                df = self.archive.with_columns([
+                    pl.col("AllPagesText").str.extract(r'(?s)Images(.+)END OF THE REPORT').str.replace(r'\n Pages\s*','').alias("Images")
+                ])
+                df = df.select(
+                    pl.col("CaseNumber"),
+                    pl.col("Images").apply(lambda x: re.split(r'(\d\d?:\d\d:\d\d [AP]M)', x))
                 )
-                images = images.explode("Images")
-                images = images.filter(pl.col("Images").str.contains(r"[A-Za-z0-9]"))
-                images = images.select(
-                    [
-                        pl.col("CaseNumber"),
-                        pl.col("Images")
-                        .str.replace_all(r"[A-Z][a-z]+", " ")
-                        .str.replace_all(r"[\s\:]+", " ")
-                        .str.strip(),
-                    ]
+                df = df.select(
+                    pl.col("CaseNumber"),
+                    pl.col("Images").apply(lambda x: x[0::2][0:-1]).alias("Row"),
+                    pl.col("Images").apply(lambda x: x[1::2]).alias("Time")
                 )
-                images = images.select(
-                    [
-                        pl.col("CaseNumber"),
-                        pl.col("Images").str.extract(r'(\d\d?/\d\d?/\d\d\d\d) (\d\d? \d\d? \d\d? [A|P]M)', group_index=1).str.to_date('%-m/%-d/%Y', strict=False).alias("Date"),
-                        pl.col("Images").str.extract(r'(\d\d?/\d\d?/\d\d\d\d) (\d\d? \d\d? \d\d? [A|P]M)', group_index=2).alias("Time"),
-                        pl.col("Images").str.extract(r'^\d\s.+?\s(\d)').cast(pl.Int64, strict=False).alias("Doc#"),
-                        pl.col("Images").str.extract(r'^\d\s(.+?)\s\d').alias("Title"),
-                        pl.col("Images").str.extract(r'^\d\s.+?\s\d\s(.+?)\s\d\d?/\d\d?/\d\d\d\d').alias("Description"),
-                        pl.col("Images").str.extract(r'^(\d)\s').cast(pl.Int64, strict=False).alias("Pages")
-                    ])
-                images = images.with_columns(
-                    pl.concat_str([
-                        pl.col("Time").str.extract(r'^(\d\d?)'),
-                        pl.lit(":"),
-                        pl.col("Time").str.extract(r'\d\d? (\d\d)'),
-                        pl.lit(":"),
-                        pl.col("Time").str.extract(r'\d\d? \d\d (\d\d [A|P]M)')
-                    ]).alias("Time")
-                )
-                images = images.filter(pl.col("Date").is_null().is_not())
-                images = images.fill_null('')
-            self._images = images
+                df = df.explode("Row", "Time")
+                df = df.with_columns([
+                    pl.col("Row").str.replace(r'..Alacourt\.com \d\d?/\d\d?/\d\d\d\d \d+','').str.strip(),
+                    pl.col("Time").str.strip()
+                ])
+                df = df.select([
+                    pl.col("CaseNumber"),
+                    pl.col("Row").str.extract(r'(\d\d?/\d\d?/\d\d\d\d)').str.to_date('%m/%d/%Y', strict=False).alias("Date"),
+                    pl.col("Time"),
+                    pl.col("Row").str.extract(r'\d+ [^0-9]+ (\d+)').alias("Doc#"),
+                    pl.col("Row").str.extract(r'\d+ ([^0-9]+)').str.strip().alias("Title"),
+                    pl.col("Row").str.extract(r'(?s)\d+ [^0-9]+ \d+ (.+) \d\d?/\d\d?/\d\d\d\d$').alias("Description"),
+                    pl.col("Row").str.extract(r'^(\d+)').alias("Pages")
+                ])
+                df = df.drop_nulls("Date")
+            self._images = df
             return self._images
     
     def tables(self):
         return {
             'cases': self.cases(),
-            'charges': self.charges(),
+            'filing-charges': self.filing_charges(),
+            'disposition-charges': self.disposition_charges(),
             'fees': self.fees(),
             'sentences': self.sentences(),
             'financial-history': self.financial_history(),
             'witnesses': self.witnesses(),
             'attorneys': self.attorneys(),
             'images': self.images(),
             'case-action-summary': self.case_action_summary()
@@ -2615,76 +2454,76 @@
                 pl.col("Name"),
                 pl.col("Search").alias("AIS / Unique ID")
             ])
             self._pairs = self._pairs.unique()
         if not self.is_read:
             self.read()
         cases = self.cases()
-        charges = self.charges()
+        dch = self.disposition_charges()
+        fch = self.filing_charges()
         with console.status("Creating summary..."):
             cases = cases.select("CaseNumber", "Name", "DOB", "Race", "Sex")
             cases = cases.with_columns(
                 [
                     pl.col("Race").cast(pl.Utf8, strict=False),
                     pl.col("Sex").cast(pl.Utf8, strict=False),
                 ]
             )
-            fch = charges.filter(pl.col("Filing"))
             fch = fch.join(self._pairs, on="Name", how="outer")
             fch = fch.groupby("AIS / Unique ID").all()
             fch = fch.select(
                 [
                     pl.col("AIS / Unique ID"),
-                    pl.col("CERVDisqCharge").list.count_match(True).alias("CERVChargesCount"),
-                    pl.col("PardonDisqCharge")
+                    pl.col("CERVCharge").list.count_match(True).alias("CERVChargesCount"),
+                    pl.col("PardonToVoteCharge")
                     .list.count_match(True)
                     .alias("PardonToVoteChargesCount"),
-                    pl.col("PermanentDisqCharge")
+                    pl.col("PermanentCharge")
                     .list.count_match(True)
-                    .alias("PermanentDisqChargesCount"),
+                    .alias("PermanentChargesCount"),
                     pl.col("ChargesSummary").list.join(", ")
                     .str.replace_all(r"null,?", "")
                     .str.strip()
                     .str.replace(r",$", "")
                     .str.replace_all(r"\s+", " ")
                     .alias("FilingCharges"),
 
                 ]
             )
-            conv = charges.filter(pl.col("Disposition") & pl.col("Conviction"))
+            conv = dch.filter("Conviction")
             conv = conv.join(self._pairs, on="Name", how="outer")
             conv = conv.groupby("AIS / Unique ID").all()
             conv = conv.select(
                 [
                     pl.col("AIS / Unique ID"),
                     pl.col("Conviction")
                     .list.count_match(True)
                     .alias("ConvictionCount"),
-                    pl.col("CERVDisqConviction")
+                    pl.col("CERVConviction")
                     .list.count_match(True)
                     .alias("CERVConvictionCount"),
-                    pl.col("PardonDisqConviction")
+                    pl.col("PardonToVoteConviction")
                     .list.count_match(True)
                     .alias("PardonToVoteConvictionCount"),
-                    pl.col("PermanentDisqConviction")
+                    pl.col("PermanentConviction")
                     .list.count_match(True)
-                    .alias("PermanentDisqConvictionCount"),
+                    .alias("PermanentConvictionCount"),
                     pl.col("PaymentToRestore").list.mean(),
                     pl.col("ChargesSummary").list.join(", ")
                     .str.replace_all(r"null,?", "")
                     .str.strip()
                     .str.replace(r",$", "")
                     .str.replace_all(r"\s+", " ")
                     .alias("Convictions"),
                 ]
             )
-            vrr = charges.filter(
-                pl.col("CERVDisqConviction")
-                | pl.col("PardonDisqConviction")
-                | pl.col("PermanentDisqConviction")
+            vrr = dch.filter(
+                pl.col("CERVConviction")
+                | pl.col("PardonToVoteConviction")
+                | pl.col("PermanentConviction")
             )
             vrr = vrr.join(self._pairs, on="Name", how="outer")
             vrr = vrr.groupby("AIS / Unique ID").all()
             vrr = vrr.select(
                 [
                     pl.col("AIS / Unique ID"),
                     pl.col("ChargesSummary").list.join(", ")
@@ -2708,24 +2547,24 @@
                     .str.replace(r",$", "")
                     .str.replace_all(r"\s+", " ")
                     .alias("Cases")
                 ]
             )
             cases = cases.with_columns(
                 [
-                    pl.when(pl.col("CERVConvictionCount").eq(0) & pl.col("PardonToVoteConvictionCount").eq(0) & pl.col("PermanentDisqConvictionCount").eq(0) & pl.col("Cases").str.lengths().gt(0))
+                    pl.when(pl.col("CERVConvictionCount").eq(0) & pl.col("PardonToVoteConvictionCount").eq(0) & pl.col("PermanentConvictionCount").eq(0) & pl.col("Cases").str.lengths().gt(0))
                     .then(True).otherwise(False)
                     .alias("EligibleToVote"),
-                    pl.when(pl.col("CERVConvictionCount").gt(0) & pl.col("PardonToVoteConvictionCount").eq(0) & pl.col("PermanentDisqConvictionCount").eq(0))
+                    pl.when(pl.col("CERVConvictionCount").gt(0) & pl.col("PardonToVoteConvictionCount").eq(0) & pl.col("PermanentConvictionCount").eq(0))
                     .then(True).otherwise(False)
                     .alias("NeedsCERV"),
-                    pl.when(pl.col("PardonToVoteConvictionCount") > 0 & pl.col("PermanentDisqConvictionCount").eq(0))
+                    pl.when(pl.col("PardonToVoteConvictionCount") > 0 & pl.col("PermanentConvictionCount").eq(0))
                     .then(True).otherwise(False)
                     .alias("NeedsPardon"),
-                    pl.when(pl.col("PermanentDisqConvictionCount").gt(0))
+                    pl.when(pl.col("PermanentConvictionCount").gt(0))
                     .then(True).otherwise(False)
                     .alias("PermanentlyDisqualified")
                 ]
             )
             cases = cases.with_columns(
                 [
                     pl.when(pl.col("Cases").str.lengths().eq(0))
@@ -2755,16 +2594,16 @@
                     pl.col("NeedsPardon"),
                     pl.col("PermanentlyDisqualified"),
                     pl.col("ConvictionCount"),
                     pl.col("CERVChargesCount"),
                     pl.col("CERVConvictionCount"),
                     pl.col("PardonToVoteChargesCount"),
                     pl.col("PardonToVoteConvictionCount"),
-                    pl.col("PermanentDisqChargesCount"),
-                    pl.col("PermanentDisqConvictionCount"),
+                    pl.col("PermanentChargesCount"),
+                    pl.col("PermanentConvictionCount"),
                     pl.col("DisqualifyingConvictions"),
                     pl.col("Convictions"),
                     pl.col("FilingCharges"),
                     pl.col("Cases")
                 ]
             )
             cases = cases.sort("Name")
@@ -2819,15 +2658,16 @@
             names = names.filter(pl.col("Name") != "")
         self._pairs_template = names
         return self._pairs_template
 
     def write_tables(self, path):
         all_tables = {
             'cases': self._cases, 
-            'charges': self._charges, 
+            'filing-charges': self._filing_charges,
+            'disposition-charges': self._disposition_charges, 
             'fees': self._fees, 
             'sentences': self._sentences, 
             'financial-history': self._financial_history, 
             'witnesses': self._witnesses, 
             'attorneys': self._attorneys, 
             'images': self._images, 
             'case-action-summary': self._case_action_summary
@@ -2847,24 +2687,25 @@
         write({'archive': out}, path, log=True)
         return out
 
 ## COMMAND LINE INTERFACE
 
 @app.command(no_args_is_help=True)
 def party_search(
-    queue_path: Annotated[Path, typer.Argument(help="Path to queue table with one or more columns: Name, Party Type, SSN, DOB, County, Division, Case Year, Filed Before, Filed After, No Records.", show_default=False)],
+    queue_path: Annotated[Path, typer.Argument(help="Path to queue table with one or more columns: \'Name\', \'Party Type\', \'SSN\', \'DOB\', \'County\', \'Division\', \'Case Year\', \'Filed Before\', \'Filed After\', \'No Records\'.", show_default=False)],
     output_path: Annotated[Path, typer.Argument(help="Path to output results table. Will attempt to append to existing table at output path.", show_default=False)],
     customer_ID: Annotated[str, typer.Option("--customer-id", "-c", help="Customer ID for Alacourt login.", prompt="Customer ID", show_default=False)],
     user_ID: Annotated[str, typer.Option("--user-id", "-u", help="User ID for Alacourt login.", prompt="User ID", show_default=False)],
     password: Annotated[str, typer.Option("--password", "-p", help="Password for Alacourt login.", prompt="Password", hide_input=True, show_default=False)],
     criminal_only: Annotated[bool, typer.Option("--criminal-only", help="Only search criminal cases.", show_default=False)] = False,
-    show_browser: Annotated[bool, typer.Option("--show-browser", help="Show browser window while working.", show_default=False)] = False
+    show_browser: Annotated[bool, typer.Option("--show-browser", help="Show browser window while working.", show_default=False)] = False,
+    verbose: Annotated[bool, typer.Option("--verbose", help="Print detailed logs while working.", show_default=False)] = False
 ):
     """
-    Collect results from Alacourt Party Search into a table at `output_path`. Input `queue_path` table from .xls(x), .csv, .json, or .parquet with columns corresponding to Alacourt Party Search fields: Name, Party Type, SSN, DOB, County, Division, Case Year, Filed Before, Filed After, No Records.
+    Collect results from Alacourt Party Search into a table at `output_path`. Input `queue_path` table from .xls(x), .csv, .json, or .parquet with columns corresponding to Alacourt Party Search fields: 'Name', 'Party Type', 'SSN', 'DOB', 'County', 'Division', 'Case Year', 'Filed Before', 'Filed After', 'No Records'.
     """ 
     queue_path = os.path.abspath(queue_path)
     output_path = os.path.abspath(output_path)
     headless = not show_browser
 
     if os.path.splitext(queue_path)[1] not in (".xls", ".xlsx", ".csv", ".json", ".parquet"):
         raise Exception("Queue path file extension not supported. Retry with .xls, .xlsx, .csv, .json, or .parquet.")
@@ -2873,20 +2714,21 @@
 
     driver = AlacourtDriver(headless=headless)
     driver.login(customer_ID, user_ID, password)
     driver.start_party_search_queue(queue_path, output_path, criminal_only)
 
 @app.command(no_args_is_help=True)
 def fetch_cases(
-    queue_path: Annotated[Path, typer.Argument(help="Path to queue table with `CaseNumber` column.", show_default=False)],
+    queue_path: Annotated[Path, typer.Argument(help="Path to queue table with \'Case Number\' column.", show_default=False)],
     output_path: Annotated[Path, typer.Argument(help="Path to output directory. PDFs will populate directory as they download.", show_default=False)],
     customer_ID: Annotated[str, typer.Option("--customer-id", "-c", help="Customer ID for Alacourt login.", prompt="Customer ID", show_default=False)],
     user_ID: Annotated[str, typer.Option("--user-id", "-u", help="User ID for Alacourt login.", prompt="User ID", show_default=False)],
     password: Annotated[str, typer.Option("--password", "-p", help="Password for Alacourt login.", prompt="Password", hide_input=True, show_default=False)],
-    show_browser: Annotated[bool, typer.Option("--show-browser", help="Show browser window while working.", show_default=False)] = False
+    show_browser: Annotated[bool, typer.Option("--show-browser", help="Show browser window while working.", show_default=False)] = False,
+    verbose: Annotated[bool, typer.Option("--verbose", help="Print detailed logs while working.", show_default=False)] = False
 ):
     """
     From a queue table with `CaseNumber` column, download case detail PDFs to directory at `output_path`.
     """
     queue_path = os.path.abspath(queue_path)
     output_path = os.path.abspath(output_path)
     headless = not show_browser
@@ -2894,15 +2736,15 @@
     if os.path.splitext(queue_path)[1] not in (".xls", ".xlsx", ".csv", ".json", ".parquet"):
         raise Exception("Queue path file extension not supported. Retry with .xls, .xlsx, .csv, .json, or .parquet.")
     if not os.path.isdir(output_path):
         raise Exception("Output path must be valid directory.")
 
     driver = AlacourtDriver(output_path, headless=headless)
     driver.login(customer_ID, user_ID, password)
-    driver.start_case_number_queue(queue_path)
+    driver.start_case_number_queue(queue_path, verbose=verbose)
 
 @app.command(no_args_is_help=True)
 def crawl_adoc(
     output_path: Annotated[Path, typer.Argument(help="Path to output table (.xls, .xlsx, .csv, .json, .parquet).", show_default=False)],
     show_browser: Annotated[bool, typer.Option("--show-browser", help="Show browser window while working.", show_default=False)] = False
 ):
     """
@@ -2914,25 +2756,26 @@
     driver = ADOCDriver(output_path, headless)
     driver.crawl(output_path)
 
 @app.command(no_args_is_help=True)
 def search_adoc(
     queue_path: Annotated[Path, typer.Argument(help="Path to queue table with \'First Name\', \'Last Name\', and \'AIS\' columns.", show_default=False)],
     output_path: Annotated[Path, typer.Argument(help="Path to output table (.xls, .xlsx, .csv, .json, .parquet).", show_default=False)],
-    show_browser: Annotated[bool, typer.Option("--show-browser", help="Show browser window while working.", show_default=False)] = False
+    show_browser: Annotated[bool, typer.Option("--show-browser", help="Show browser window while working.", show_default=False)] = False,
+    verbose: Annotated[bool, typer.Option("--verbose", help="Print detailed logs while working.", show_default=False)] = False
 ):
     """
     Search ADOC using queue with First Name, Last Name, and AIS columns to retrieve sentencing information from ADOC. Record table to `output_path`.
     """
     queue_path = os.path.abspath(queue_path)
     output_path = os.path.abspath(output_path)
     headless = not show_browser
 
     driver = ADOCDriver(output_path, headless)
-    driver.start_queue(queue_path, output_path)
+    driver.start_queue(queue_path, output_path, verbose=verbose)
 
 @app.command(no_args_is_help=True)
 def make_archive(
     directory_path: Annotated[Path, typer.Argument(help="Path to PDF case directory.", show_default=False)],
     output_path: Annotated[Path, typer.Argument(help="Path to output archive (recommend .parquet).", show_default=False)]
 ):
     """
@@ -2944,36 +2787,38 @@
     cases = Cases(str(directory_path))
     cases.write_archive(str(output_path))
 
 @app.command(no_args_is_help=True)
 def make_table(
     input_path: Annotated[Path, typer.Argument(help="Path to input case directory or archive.", show_default=False)],
     output_path: Annotated[Path, typer.Argument(help="Path to output table (.xls, .xlsx, .csv, .json, .parquet). `All` table export must output to .xls or .xlsx.", show_default=False)],
-    table: Annotated[str, typer.Option("--table", "-t", help="Output table selection: all, cases, charges, fees, attorneys, case-action-summary, financial-history, images, sentences, settings, witnesses.", show_default=True)] = "all"
+    table: Annotated[str, typer.Option("--table", "-t", help="Output table selection: all, cases, filing-charges, disposition-charges, fees, attorneys, case-action-summary, financial-history, images, sentences, settings, witnesses.", show_default=True)] = "all"
 ):
     """
     Create table at `output_path` from archive or directory at `input_path`.
     """
     input_path = os.path.abspath(input_path)
     output_path = os.path.abspath(output_path)
 
     if table == "all" and os.path.splitext(output_path)[1] not in (".xls",".xlsx"):
-        raise Exception("Must select a table to export using --table flag. Options: cases, charges, fees, attorneys, case-action-summary, financial-history, images, sentences, settings, witnesses.")
+        raise Exception("Must select a table to export using --table flag. Options: cases, filing-charges, disposition-charges, fees, attorneys, case-action-summary, financial-history, images, sentences, settings, witnesses.")
 
     cases = Cases(str(input_path))
     cases.read()
 
     if table == "all":
         output = cases.tables()
     elif table == "cases":
         output = cases.cases()
     elif table == "fees":
         output = cases.fees()
-    elif table == "charges":
-        output = cases.charges()
+    elif table == "filing-charges":
+        output = cases.filing_charges()
+    elif table == "disposition-charges":
+        output = casees.disposition_charges()
     elif table == "attorneys":
         output = cases.attorneys()
     elif table == "case-action-summary":
         output = cases.case_action_summary()
     elif table == "financial-history":
         output = cases.financial_history()
     elif table == "images":
@@ -2981,15 +2826,15 @@
     elif table == "sentences":
         output = cases.sentences()
     elif table == "settings":
         output = cases.settings()
     elif table == "witnesses":
         output = cases.witnesses()
     else:
-        raise Exception("Invalid table selection. Options: all, cases, charges, fees, attorneys, case-action-summary, financial-history, images, sentences, settings, witnesses.")
+        raise Exception("Invalid table selection. Options: all, cases, filing-charges, disposition-charges, fees, attorneys, case-action-summary, financial-history, images, sentences, settings, witnesses.")
 
     write(output, output_path, log=True)
 
 @app.command(no_args_is_help=True)
 def make_summary(
     input_path: Annotated[Path, typer.Argument(help="Path to input case directory or archive.", show_default=False)],
     pairs_path: Annotated[Path, typer.Argument(help="Path to filled pairs template or party search results table.", show_default=False)],
```

### Comparing `alacorder-81.0.1/pyproject.toml` & `alacorder-81.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "81.0.1"
+version = "81.0.2"
 description = "Alacorder retrieves case detail PDFs from Alacourt.com and processes them into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 typer = {extras = ["all"], version = "^0.9.0"}
```

### Comparing `alacorder-81.0.1/PKG-INFO` & `alacorder-81.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 81.0.1
+Version: 81.0.2
 Summary: Alacorder retrieves case detail PDFs from Alacourt.com and processes them into data tables suitable for research purposes.
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

