# Comparing `tmp/gitstats_abilian-1.0.3.tar.gz` & `tmp/gitstats_abilian-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitstats_abilian-1.0.3.tar", max compression
+gzip compressed data, was "gitstats_abilian-1.0.4.tar", max compression
```

## Comparing `gitstats_abilian-1.0.3.tar` & `gitstats_abilian-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      546 2023-07-27 07:56:57.995107 gitstats_abilian-1.0.3/README.md
--rw-r--r--   0        0        0      446 2023-07-27 08:23:13.949807 gitstats_abilian-1.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-27 06:49:17.000000 gitstats_abilian-1.0.3/src/gitstats/__init__.py
--rw-r--r--   0        0        0       73 2023-07-27 06:45:33.000000 gitstats_abilian-1.0.3/src/gitstats/assets/arrow-down.gif
--rw-r--r--   0        0        0       71 2023-07-27 06:45:33.000000 gitstats_abilian-1.0.3/src/gitstats/assets/arrow-none.gif
--rw-r--r--   0        0        0       73 2023-07-27 06:45:33.000000 gitstats_abilian-1.0.3/src/gitstats/assets/arrow-up.gif
--rw-r--r--   0        0        0     1645 2023-07-27 06:45:33.000000 gitstats_abilian-1.0.3/src/gitstats/assets/gitstats.css
--rw-r--r--   0        0        0     9562 2023-07-27 06:45:33.000000 gitstats_abilian-1.0.3/src/gitstats/assets/sortable.js
--rw-r--r--   0        0        0    25839 2023-07-27 08:13:13.899988 gitstats_abilian-1.0.3/src/gitstats/collector.py
--rw-r--r--   0        0        0      821 2023-07-27 07:48:16.895377 gitstats_abilian-1.0.3/src/gitstats/config.py
--rwxr-xr-x   0        0        0     2930 2023-07-27 08:09:20.807774 gitstats_abilian-1.0.3/src/gitstats/gitstats.py
--rw-r--r--   0        0        0      140 2023-07-27 07:26:27.359393 gitstats_abilian-1.0.3/src/gitstats/main.py
--rw-r--r--   0        0        0    30085 2023-07-27 07:44:44.667624 gitstats_abilian-1.0.3/src/gitstats/report.py
--rw-r--r--   0        0        0     3313 2023-07-27 07:45:48.884403 gitstats_abilian-1.0.3/src/gitstats/utils.py
--rw-r--r--   0        0        0      714 2023-07-27 08:06:34.872976 gitstats_abilian-1.0.3/src/gitstats/version.py
--rw-r--r--   0        0        0      941 1970-01-01 00:00:00.000000 gitstats_abilian-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      546 2023-07-27 07:56:57.995107 gitstats_abilian-1.0.4/README.md
+-rw-r--r--   0        0        0     1873 2023-07-27 08:35:44.961796 gitstats_abilian-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-27 06:49:17.000000 gitstats_abilian-1.0.4/src/gitstats/__init__.py
+-rw-r--r--   0        0        0       73 2023-07-27 06:45:33.000000 gitstats_abilian-1.0.4/src/gitstats/assets/arrow-down.gif
+-rw-r--r--   0        0        0       71 2023-07-27 06:45:33.000000 gitstats_abilian-1.0.4/src/gitstats/assets/arrow-none.gif
+-rw-r--r--   0        0        0       73 2023-07-27 06:45:33.000000 gitstats_abilian-1.0.4/src/gitstats/assets/arrow-up.gif
+-rw-r--r--   0        0        0     1645 2023-07-27 06:45:33.000000 gitstats_abilian-1.0.4/src/gitstats/assets/gitstats.css
+-rw-r--r--   0        0        0     9562 2023-07-27 06:45:33.000000 gitstats_abilian-1.0.4/src/gitstats/assets/sortable.js
+-rw-r--r--   0        0        0    25824 2023-07-27 08:34:37.890540 gitstats_abilian-1.0.4/src/gitstats/collector.py
+-rw-r--r--   0        0        0      821 2023-07-27 07:48:16.895377 gitstats_abilian-1.0.4/src/gitstats/config.py
+-rwxr-xr-x   0        0        0     2930 2023-07-27 08:09:20.807774 gitstats_abilian-1.0.4/src/gitstats/gitstats.py
+-rw-r--r--   0        0        0      140 2023-07-27 07:26:27.359393 gitstats_abilian-1.0.4/src/gitstats/main.py
+-rw-r--r--   0        0        0    30145 2023-07-27 08:34:37.896319 gitstats_abilian-1.0.4/src/gitstats/report.py
+-rw-r--r--   0        0        0     3313 2023-07-27 08:26:56.047879 gitstats_abilian-1.0.4/src/gitstats/utils.py
+-rw-r--r--   0        0        0      714 2023-07-27 08:06:34.872976 gitstats_abilian-1.0.4/src/gitstats/version.py
+-rw-r--r--   0        0        0      941 1970-01-01 00:00:00.000000 gitstats_abilian-1.0.4/PKG-INFO
```

### Comparing `gitstats_abilian-1.0.3/README.md` & `gitstats_abilian-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `gitstats_abilian-1.0.3/src/gitstats/assets/gitstats.css` & `gitstats_abilian-1.0.4/src/gitstats/assets/gitstats.css`

 * *Files identical despite different names*

### Comparing `gitstats_abilian-1.0.3/src/gitstats/assets/sortable.js` & `gitstats_abilian-1.0.4/src/gitstats/assets/sortable.js`

 * *Files identical despite different names*

### Comparing `gitstats_abilian-1.0.3/src/gitstats/collector.py` & `gitstats_abilian-1.0.4/src/gitstats/collector.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,23 +3,17 @@
 import pickle
 import re
 import time
 import zlib
 from multiprocessing import Pool
 
 from .config import conf
-from .utils import (
-    getkeyssortedbyvaluekey,
-    getpipeoutput,
-    getlogrange,
-    getnumoffilesfromrev,
-    getcommitrange,
-    getnumoflinesinblob,
-    getstatsummarycounts,
-)
+from .utils import (getcommitrange, getkeyssortedbyvaluekey, getlogrange,
+                    getnumoffilesfromrev, getnumoflinesinblob, getpipeoutput,
+                    getstatsummarycounts)
 
 
 class DataCollector:
     """Manages data collection from a revision control repository."""
 
     dir: str
     projectname: str
@@ -42,17 +36,15 @@
         #   first_commit_stamp,
         #   last_commit_stamp,
         #   last_active_day,
         #   active_days,
         #   lines_added,
         #   lines_removed.
         # }
-        self.authors = (
-            {}
-        )
+        self.authors = {}
 
         self.total_commits = 0
         self.total_files = 0
         self.authors_by_commits = 0
 
         # domains
         self.domains = {}  # domain -> commits
```

### Comparing `gitstats_abilian-1.0.3/src/gitstats/config.py` & `gitstats_abilian-1.0.4/src/gitstats/config.py`

 * *Files identical despite different names*

### Comparing `gitstats_abilian-1.0.3/src/gitstats/gitstats.py` & `gitstats_abilian-1.0.4/src/gitstats/gitstats.py`

 * *Files identical despite different names*

### Comparing `gitstats_abilian-1.0.3/src/gitstats/report.py` & `gitstats_abilian-1.0.4/src/gitstats/report.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+import contextlib
 import datetime
 import glob
 import os
 import shutil
 import time
 from pathlib import Path
 
-from .config import conf, WEEKDAYS, GNUPLOT_COMMON, gnuplot_cmd
-from .utils import getkeyssortedbyvaluekey, getkeyssortedbyvalues, getpipeoutput
-from .version import getversion, getgitversion, getgnuplotversion
+from .config import GNUPLOT_COMMON, WEEKDAYS, conf, gnuplot_cmd
+from .utils import (getkeyssortedbyvaluekey, getkeyssortedbyvalues,
+                    getpipeoutput)
+from .version import getgitversion, getgnuplotversion, getversion
 
 
 class ReportCreator:
     """Creates the actual report based on given data."""
 
     def __init__(self):
         pass
@@ -69,20 +71,20 @@
             "<dt>Generated</dt><dd>%s (in %d seconds)</dd>"
             % (
                 datetime.datetime.now().strftime(format),
                 time.time() - data.getStampCreated(),
             )
         )
         f.write(
-            '<dt>Generator</dt><dd><a href="http://gitstats.sourceforge.net/">GitStats</a> (version %s), %s, %s</dd>'
-            % (getversion(), getgitversion(), getgnuplotversion())
+            '<dt>Generator</dt><dd><a href="http://gitstats.sourceforge.net/">GitStats</a> (version {}), {}, {}</dd>'.format(
+                getversion(), getgitversion(), getgnuplotversion()
+            )
         )
         f.write(
-            "<dt>Report Period</dt><dd>%s to %s</dd>"
-            % (
+            "<dt>Report Period</dt><dd>{} to {}</dd>".format(
                 data.getFirstCommitDate().strftime(format),
                 data.getLastCommitDate().strftime(format),
             )
         )
         f.write(
             "<dt>Age</dt><dd>%d days, %d active days (%3.2f%%)</dd>"
             % (
@@ -93,24 +95,22 @@
         )
         f.write(f"<dt>Total Files</dt><dd>{data.getTotalFiles()}</dd>")
         f.write(
             "<dt>Total Lines of Code</dt><dd>%s (%d added, %d removed)</dd>"
             % (data.getTotalLOC(), data.total_lines_added, data.total_lines_removed)
         )
         f.write(
-            "<dt>Total Commits</dt><dd>%s (average %.1f commits per active day, %.1f per all days)</dd>"
-            % (
+            "<dt>Total Commits</dt><dd>{} (average {:.1f} commits per active day, {:.1f} per all days)</dd>".format(
                 data.getTotalCommits(),
                 float(data.getTotalCommits()) / len(data.getActiveDays()),
                 float(data.getTotalCommits()) / data.getCommitDeltaDays(),
             )
         )
         f.write(
-            "<dt>Authors</dt><dd>%s (average %.1f commits per author)</dd>"
-            % (
+            "<dt>Authors</dt><dd>{} (average {:.1f} commits per author)</dd>".format(
                 data.getTotalAuthors(),
                 (1.0 * data.getTotalCommits()) / data.getTotalAuthors(),
             )
         )
         f.write("</dl>")
 
         f.write("</body>\n</html>")
@@ -284,15 +284,15 @@
         f.write('<img src="month_of_year.png" alt="Month of Year">')
 
         # Commits by year/month
         f.write(html_header(2, "Commits by year/month"))
         f.write(
             '<div class="vtable"><table><tr><th>Month</th><th>Commits</th><th>Lines added</th><th>Lines removed</th></tr>'
         )
-        for yymm in reversed(sorted(data.commits_by_month.keys())):
+        for yymm in sorted(data.commits_by_month.keys(), reverse=True):
             f.write(
                 "<tr><td>%s</td><td>%d</td><td>%d</td><td>%d</td></tr>"
                 % (
                     yymm,
                     data.commits_by_month.get(yymm, 0),
                     data.lines_added_by_month.get(yymm, 0),
                     data.lines_removed_by_month.get(yymm, 0),
@@ -306,15 +306,15 @@
         fg.close()
 
         # Commits by year
         f.write(html_header(2, "Commits by Year"))
         f.write(
             '<div class="vtable"><table><tr><th>Year</th><th>Commits (% of all)</th><th>Lines added</th><th>Lines removed</th></tr>'
         )
-        for yy in reversed(sorted(data.commits_by_year.keys())):
+        for yy in sorted(data.commits_by_year.keys(), reverse=True):
             f.write(
                 "<tr><td>%s</td><td>%d (%.2f%%)</td><td>%d</td><td>%d</td></tr>"
                 % (
                     yy,
                     data.commits_by_year.get(yy, 0),
                     (100.0 * data.commits_by_year.get(yy, 0)) / data.getTotalCommits(),
                     data.lines_added_by_year.get(yy, 0),
@@ -424,15 +424,15 @@
         for author in self.authors_to_plot:
             lines_by_authors[author] = 0
             commits_by_authors[author] = 0
         for stamp in sorted(data.changes_by_date_by_author.keys()):
             fgl.write("%d" % stamp)
             fgc.write("%d" % stamp)
             for author in self.authors_to_plot:
-                if author in data.changes_by_date_by_author[stamp].keys():
+                if author in data.changes_by_date_by_author[stamp]:
                     lines_by_authors[author] = data.changes_by_date_by_author[stamp][
                         author
                     ]["lines_added"]
                     commits_by_authors[author] = data.changes_by_date_by_author[stamp][
                         author
                     ]["commits"]
                 fgl.write(" %d" % lines_by_authors[author])
@@ -445,15 +445,15 @@
         # Authors :: Author of Month
         f.write(html_header(2, "Author of Month"))
         f.write('<table class="sortable" id="aom">')
         f.write(
             '<tr><th>Month</th><th>Author</th><th>Commits (%%)</th><th class="unsortable">Next top %d</th><th>Number of authors</th></tr>'
             % conf["authors_top"]
         )
-        for yymm in reversed(sorted(data.author_of_month.keys())):
+        for yymm in sorted(data.author_of_month.keys(), reverse=True):
             authordict = data.author_of_month[yymm]
             authors = getkeyssortedbyvalues(authordict)
             authors = list(authors)
             authors.reverse()
             commits = data.author_of_month[yymm][authors[0]]
             next = ", ".join(authors[1 : conf["authors_top"] + 1])
             f.write(
@@ -472,15 +472,15 @@
         f.write("</table>")
 
         f.write(html_header(2, "Author of Year"))
         f.write(
             '<table class="sortable" id="aoy"><tr><th>Year</th><th>Author</th><th>Commits (%%)</th><th class="unsortable">Next top %d</th><th>Number of authors</th></tr>'
             % conf["authors_top"]
         )
-        for yy in reversed(sorted(data.author_of_year.keys())):
+        for yy in sorted(data.author_of_year.keys(), reverse=True):
             authordict = data.author_of_year[yy]
             authors = getkeyssortedbyvalues(authordict)
             authors = list(authors)
             authors.reverse()
             commits = data.author_of_year[yy][authors[0]]
             next = ", ".join(authors[1 : conf["authors_top"] + 1])
             f.write(
@@ -530,21 +530,20 @@
         self.printHeader(f)
         f.write("<h1>Files</h1>")
         self.printNav(f)
 
         f.write("<dl>\n")
         f.write("<dt>Total files</dt><dd>%d</dd>" % data.getTotalFiles())
         f.write("<dt>Total lines</dt><dd>%d</dd>" % data.getTotalLOC())
-        try:
+        with contextlib.suppress(ZeroDivisionError):
             f.write(
                 "<dt>Average file size</dt><dd>%.2f bytes</dd>"
                 % (float(data.getTotalSize()) / data.getTotalFiles())
             )
-        except ZeroDivisionError:
-            pass
+
         f.write("</dl>\n")
 
         # Files :: File count by date
         f.write(html_header(2, "File count by date"))
 
         # use set to get rid of duplicate/unnecessary entries
         files_by_date = set()
@@ -554,15 +553,15 @@
                 % (
                     datetime.datetime.fromtimestamp(stamp).strftime("%Y-%m-%d"),
                     data.files_by_stamp[stamp],
                 )
             )
 
         fg = open(path + "/files_by_date.dat", "w")
-        for line in sorted(list(files_by_date)):
+        for line in sorted(files_by_date):
             fg.write(f"{line}\n")
         # for stamp in sorted(data.files_by_stamp.keys()):
         # 	fg.write('%s %d\n' % (datetime.datetime.fromtimestamp(stamp).strftime('%Y-%m-%d'), data.files_by_stamp[stamp]))
         fg.close()
 
         f.write('<img src="files_by_date.png" alt="Files by Date">')
 
@@ -633,17 +632,19 @@
                 % (1.0 * data.getTotalCommits() / len(data.tags))
             )
         f.write("</dl>")
 
         f.write('<table class="tags">')
         f.write("<tr><th>Name</th><th>Date</th><th>Commits</th><th>Authors</th></tr>")
         # sort the tags by date desc
-        tags_sorted_by_date_desc = map(
-            lambda el: el[1],
-            reversed(sorted(map(lambda el: (el[1]["date"], el[0]), data.tags.items()))),
+        tags_sorted_by_date_desc = (
+            el[1]
+            for el in sorted(
+                ((el[1]["date"], el[0]) for el in data.tags.items()), reverse=True
+            )
         )
         for tag in tags_sorted_by_date_desc:
             authorinfo = []
             self.authors_by_commits = getkeyssortedbyvalues(data.tags[tag]["authors"])
             self.authors_by_commits2 = list(self.authors_by_commits)
             self.authors_by_commits2.reverse()
             for i in self.authors_by_commits2:
```

### Comparing `gitstats_abilian-1.0.3/src/gitstats/utils.py` & `gitstats_abilian-1.0.4/src/gitstats/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import re
 import subprocess
 import sys
 import time
 
-from .config import conf, ON_LINUX, exectime_external
+from .config import ON_LINUX, conf, exectime_external
 
 
 def getpipeoutput(cmds, quiet=(not conf["verbose"]), stream=sys.stdout):
     """
     Standardised method of calling linux commands.
     :param cmds: Command to execute
     :param quiet: Prints commands on standard output if True.
```

### Comparing `gitstats_abilian-1.0.3/src/gitstats/version.py` & `gitstats_abilian-1.0.4/src/gitstats/version.py`

 * *Files identical despite different names*

### Comparing `gitstats_abilian-1.0.3/PKG-INFO` & `gitstats_abilian-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitstats-abilian
-Version: 1.0.3
+Version: 1.0.4
 Summary: 
 Author: Stefane Fermigier
 Author-email: sf@abilian.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

