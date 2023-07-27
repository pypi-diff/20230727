# Comparing `tmp/gitstats_abilian-1.0.4.tar.gz` & `tmp/gitstats_abilian-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitstats_abilian-1.0.4.tar", max compression
+gzip compressed data, was "gitstats_abilian-1.0.5.tar", max compression
```

## Comparing `gitstats_abilian-1.0.4.tar` & `gitstats_abilian-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      546 2023-07-27 07:56:57.995107 gitstats_abilian-1.0.4/README.md
--rw-r--r--   0        0        0     1873 2023-07-27 08:35:44.961796 gitstats_abilian-1.0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-27 06:49:17.000000 gitstats_abilian-1.0.4/src/gitstats/__init__.py
--rw-r--r--   0        0        0       73 2023-07-27 06:45:33.000000 gitstats_abilian-1.0.4/src/gitstats/assets/arrow-down.gif
--rw-r--r--   0        0        0       71 2023-07-27 06:45:33.000000 gitstats_abilian-1.0.4/src/gitstats/assets/arrow-none.gif
--rw-r--r--   0        0        0       73 2023-07-27 06:45:33.000000 gitstats_abilian-1.0.4/src/gitstats/assets/arrow-up.gif
--rw-r--r--   0        0        0     1645 2023-07-27 06:45:33.000000 gitstats_abilian-1.0.4/src/gitstats/assets/gitstats.css
--rw-r--r--   0        0        0     9562 2023-07-27 06:45:33.000000 gitstats_abilian-1.0.4/src/gitstats/assets/sortable.js
--rw-r--r--   0        0        0    25824 2023-07-27 08:34:37.890540 gitstats_abilian-1.0.4/src/gitstats/collector.py
--rw-r--r--   0        0        0      821 2023-07-27 07:48:16.895377 gitstats_abilian-1.0.4/src/gitstats/config.py
--rwxr-xr-x   0        0        0     2930 2023-07-27 08:09:20.807774 gitstats_abilian-1.0.4/src/gitstats/gitstats.py
--rw-r--r--   0        0        0      140 2023-07-27 07:26:27.359393 gitstats_abilian-1.0.4/src/gitstats/main.py
--rw-r--r--   0        0        0    30145 2023-07-27 08:34:37.896319 gitstats_abilian-1.0.4/src/gitstats/report.py
--rw-r--r--   0        0        0     3313 2023-07-27 08:26:56.047879 gitstats_abilian-1.0.4/src/gitstats/utils.py
--rw-r--r--   0        0        0      714 2023-07-27 08:06:34.872976 gitstats_abilian-1.0.4/src/gitstats/version.py
--rw-r--r--   0        0        0      941 1970-01-01 00:00:00.000000 gitstats_abilian-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0      546 2023-07-27 07:56:57.995107 gitstats_abilian-1.0.5/README.md
+-rw-r--r--   0        0        0     1873 2023-07-27 08:52:03.522798 gitstats_abilian-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-27 06:49:17.000000 gitstats_abilian-1.0.5/src/gitstats/__init__.py
+-rw-r--r--   0        0        0       73 2023-07-27 06:45:33.000000 gitstats_abilian-1.0.5/src/gitstats/assets/arrow-down.gif
+-rw-r--r--   0        0        0       71 2023-07-27 06:45:33.000000 gitstats_abilian-1.0.5/src/gitstats/assets/arrow-none.gif
+-rw-r--r--   0        0        0       73 2023-07-27 06:45:33.000000 gitstats_abilian-1.0.5/src/gitstats/assets/arrow-up.gif
+-rw-r--r--   0        0        0     1645 2023-07-27 06:45:33.000000 gitstats_abilian-1.0.5/src/gitstats/assets/gitstats.css
+-rw-r--r--   0        0        0     9562 2023-07-27 06:45:33.000000 gitstats_abilian-1.0.5/src/gitstats/assets/sortable.js
+-rw-r--r--   0        0        0    25824 2023-07-27 08:51:30.962684 gitstats_abilian-1.0.5/src/gitstats/collector.py
+-rw-r--r--   0        0        0      821 2023-07-27 07:48:16.895377 gitstats_abilian-1.0.5/src/gitstats/config.py
+-rwxr-xr-x   0        0        0     2930 2023-07-27 08:09:20.807774 gitstats_abilian-1.0.5/src/gitstats/gitstats.py
+-rw-r--r--   0        0        0      140 2023-07-27 07:26:27.359393 gitstats_abilian-1.0.5/src/gitstats/main.py
+-rw-r--r--   0        0        0    30523 2023-07-27 08:51:30.968178 gitstats_abilian-1.0.5/src/gitstats/report.py
+-rw-r--r--   0        0        0     3313 2023-07-27 08:26:56.047879 gitstats_abilian-1.0.5/src/gitstats/utils.py
+-rw-r--r--   0        0        0      714 2023-07-27 08:06:34.872976 gitstats_abilian-1.0.5/src/gitstats/version.py
+-rw-r--r--   0        0        0      941 1970-01-01 00:00:00.000000 gitstats_abilian-1.0.5/PKG-INFO
```

### Comparing `gitstats_abilian-1.0.4/README.md` & `gitstats_abilian-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `gitstats_abilian-1.0.4/pyproject.toml` & `gitstats_abilian-1.0.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gitstats-abilian"
-version = "1.0.4"
+version = "1.0.5"
 description = ""
 authors = ["Stefane Fermigier <sf@abilian.com>"]
 readme = "README.md"
 packages = [{include = "gitstats", from = "src" }]
 
 [tool.poetry.scripts]
 gitstats = "gitstats.main:main"
```

### Comparing `gitstats_abilian-1.0.4/src/gitstats/assets/gitstats.css` & `gitstats_abilian-1.0.5/src/gitstats/assets/gitstats.css`

 * *Files identical despite different names*

### Comparing `gitstats_abilian-1.0.4/src/gitstats/assets/sortable.js` & `gitstats_abilian-1.0.5/src/gitstats/assets/sortable.js`

 * *Files identical despite different names*

### Comparing `gitstats_abilian-1.0.4/src/gitstats/collector.py` & `gitstats_abilian-1.0.5/src/gitstats/collector.py`

 * *Files identical despite different names*

### Comparing `gitstats_abilian-1.0.4/src/gitstats/config.py` & `gitstats_abilian-1.0.5/src/gitstats/config.py`

 * *Files identical despite different names*

### Comparing `gitstats_abilian-1.0.4/src/gitstats/gitstats.py` & `gitstats_abilian-1.0.5/src/gitstats/gitstats.py`

 * *Files identical despite different names*

### Comparing `gitstats_abilian-1.0.4/src/gitstats/report.py` & `gitstats_abilian-1.0.5/src/gitstats/report.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,37 +38,44 @@
     )
 
 
 class HTMLReportCreator(ReportCreator):
     title: str
 
     def create(self, data, path):
-        ReportCreator.create(self, data, path)
+        super().create(data, path)
         self.title = data.projectname
 
-        # copy static files. Looks in the binary directory, ../share/gitstats and /usr/share/gitstats
+        self.copy_assets(path)
+        self.create_main_report(data, path)
+        totalcommits = self.create_activity_report(data, path)
+        self.create_authors_report(data, path, totalcommits)
+        self.create_files_report(data, path)
+        self.create_lines_report(data, path)
+        self.create_tags_report(data, path)
+        self.createGraphs(path)
+
+    def copy_assets(self, path):
         for file in (
             conf["style"],
             "sortable.js",
             "arrow-up.gif",
             "arrow-down.gif",
             "arrow-none.gif",
         ):
             src_path = Path(__file__).parent / "assets" / file
             dst_path = Path(path) / file
             shutil.copyfile(src_path, dst_path)
 
+    def create_main_report(self, data, path):
         f = open(path + "/index.html", "w")
         format = "%Y-%m-%d %H:%M:%S"
         self.printHeader(f)
-
         f.write(f"<h1>GitStats - {data.projectname}</h1>")
-
         self.printNav(f)
-
         f.write("<dl>")
         f.write(f"<dt>Project name</dt><dd>{data.projectname}</dd>")
         f.write(
             "<dt>Generated</dt><dd>%s (in %d seconds)</dd>"
             % (
                 datetime.datetime.now().strftime(format),
                 time.time() - data.getStampCreated(),
@@ -108,43 +115,36 @@
         f.write(
             "<dt>Authors</dt><dd>{} (average {:.1f} commits per author)</dd>".format(
                 data.getTotalAuthors(),
                 (1.0 * data.getTotalCommits()) / data.getTotalAuthors(),
             )
         )
         f.write("</dl>")
-
         f.write("</body>\n</html>")
         f.close()
 
-        ###
-        # Activity
+    def create_activity_report(self, data, path):
         f = open(path + "/activity.html", "w")
         self.printHeader(f)
         f.write("<h1>Activity</h1>")
         self.printNav(f)
-
         # f.write('<h2>Last 30 days</h2>')
-
         # f.write('<h2>Last 12 months</h2>')
-
         # Weekly activity
         WEEKS = 32
         f.write(html_header(2, "Weekly activity"))
         f.write("<p>Last %d weeks</p>" % WEEKS)
-
         # generate weeks to show (previous N weeks from now)
         now = datetime.datetime.now()
         deltaweek = datetime.timedelta(7)
         weeks = []
         stampcur = now
         for i in range(0, WEEKS):
             weeks.insert(0, stampcur.strftime("%Y-%W"))
             stampcur -= deltaweek
-
         # top row: commits & bar
         f.write('<table class="noborders"><tr>')
         for i in range(0, WEEKS):
             commits = 0
             if weeks[i] in data.activity_by_year_week:
                 commits = data.activity_by_year_week[weeks[i]]
 
@@ -155,21 +155,19 @@
                     / data.activity_by_year_week_peak
                 )
             height = max(1, int(200 * percentage))
             f.write(
                 '<td style="text-align: center; vertical-align: bottom">%d<div style="display: block; background-color: red; width: 20px; height: %dpx"></div></td>'
                 % (commits, height)
             )
-
         # bottom row: year/week
         f.write("</tr><tr>")
         for i in range(0, WEEKS):
             f.write(f"<td>{WEEKS - i}</td>")
         f.write("</tr></table>")
-
         # Hour of Day
         f.write(html_header(2, "Hour of Day"))
         hour_of_day = data.getActivityByHourOfDay()
         f.write("<table><tr><th>Hour</th>")
         for i in range(0, 24):
             f.write("<th>%d</th>" % i)
         f.write("</tr>\n<tr><th>Commits</th>")
@@ -206,15 +204,14 @@
         fg = open(path + "/hour_of_day.dat", "w")
         for i in range(0, 24):
             if i in hour_of_day:
                 fg.write("%d %d\n" % (i + 1, hour_of_day[i]))
             else:
                 fg.write("%d 0\n" % (i + 1))
         fg.close()
-
         # Day of Week
         f.write(html_header(2, "Day of Week"))
         day_of_week = data.getActivityByDayOfWeek()
         f.write('<div class="vtable"><table>')
         f.write("<tr><th>Day</th><th>Total (%)</th></tr>")
         fp = open(path + "/day_of_week.dat", "w")
         for d in range(0, 7):
@@ -231,24 +228,21 @@
                 )
             else:
                 f.write("<td>0</td>")
             f.write("</tr>")
         f.write("</table></div>")
         f.write('<img src="day_of_week.png" alt="Day of Week">')
         fp.close()
-
         # Hour of Week
         f.write(html_header(2, "Hour of Week"))
         f.write("<table>")
-
         f.write("<tr><th>Weekday</th>")
         for hour in range(0, 24):
             f.write("<th>%d</th>" % (hour))
         f.write("</tr>")
-
         for weekday in range(0, 7):
             f.write(f"<tr><th>{WEEKDAYS[weekday]}</th>")
             for hour in range(0, 24):
                 try:
                     commits = data.activity_by_hour_of_week[weekday][hour]
                 except KeyError:
                     commits = 0
@@ -258,17 +252,15 @@
                         (float(commits) / data.activity_by_hour_of_week_busiest) * 128
                     )
                     f.write(' style="background-color: rgb(%d, 0, 0)"' % r)
                     f.write(">%d</td>" % commits)
                 else:
                     f.write("<td></td>")
             f.write("</tr>")
-
         f.write("</table>")
-
         # Month of Year
         f.write(html_header(2, "Month of Year"))
         f.write('<div class="vtable"><table>')
         f.write("<tr><th>Month</th><th>Commits (%)</th></tr>")
         fp = open(path + "/month_of_year.dat", "w")
         for mm in range(1, 13):
             commits = 0
@@ -278,15 +270,14 @@
                 "<tr><td>%d</td><td>%d (%.2f %%)</td></tr>"
                 % (mm, commits, (100.0 * commits) / data.getTotalCommits())
             )
             fp.write("%d %d\n" % (mm, commits))
         fp.close()
         f.write("</table></div>")
         f.write('<img src="month_of_year.png" alt="Month of Year">')
-
         # Commits by year/month
         f.write(html_header(2, "Commits by year/month"))
         f.write(
             '<div class="vtable"><table><tr><th>Month</th><th>Commits</th><th>Lines added</th><th>Lines removed</th></tr>'
         )
         for yymm in sorted(data.commits_by_month.keys(), reverse=True):
             f.write(
@@ -300,15 +291,14 @@
             )
         f.write("</table></div>")
         f.write('<img src="commits_by_year_month.png" alt="Commits by year/month">')
         fg = open(path + "/commits_by_year_month.dat", "w")
         for yymm in sorted(data.commits_by_month.keys()):
             fg.write(f"{yymm} {data.commits_by_month[yymm]}\n")
         fg.close()
-
         # Commits by year
         f.write(html_header(2, "Commits by Year"))
         f.write(
             '<div class="vtable"><table><tr><th>Year</th><th>Commits (% of all)</th><th>Lines added</th><th>Lines removed</th></tr>'
         )
         for yy in sorted(data.commits_by_year.keys(), reverse=True):
             f.write(
@@ -323,44 +313,39 @@
             )
         f.write("</table></div>")
         f.write('<img src="commits_by_year.png" alt="Commits by Year">')
         fg = open(path + "/commits_by_year.dat", "w")
         for yy in sorted(data.commits_by_year.keys()):
             fg.write("%d %d\n" % (yy, data.commits_by_year[yy]))
         fg.close()
-
         # Commits by timezone
         f.write(html_header(2, "Commits by Timezone"))
         f.write("<table><tr>")
         f.write("<th>Timezone</th><th>Commits</th>")
         f.write("</tr>")
         max_commits_on_tz = max(data.commits_by_timezone.values())
         for i in sorted(data.commits_by_timezone.keys(), key=lambda n: int(n)):
             commits = data.commits_by_timezone[i]
             r = 127 + int((float(commits) / max_commits_on_tz) * 128)
             f.write(
                 '<tr><th>%s</th><td style="background-color: rgb(%d, 0, 0)">%d</td></tr>'
                 % (i, r, commits)
             )
         f.write("</table>")
-
         f.write("</body></html>")
         f.close()
+        return totalcommits
 
-        ###
-        # Authors
+    def create_authors_report(self, data, path, totalcommits):
         f = open(path + "/authors.html", "w")
         self.printHeader(f)
-
         f.write("<h1>Authors</h1>")
         self.printNav(f)
-
         # Authors :: List of authors
         f.write(html_header(2, "List of Authors"))
-
         f.write('<table class="authors sortable" id="authors">')
         f.write(
             '<tr><th>Author</th><th>Commits (%)</th><th>+ lines</th><th>- lines</th><th>First commit</th><th>Last commit</th><th class="unsortable">Age</th><th>Active days</th><th># by commits</th></tr>'
         )
         for author in data.getAuthors(conf["max_authors"]):
             info = data.getAuthorInfo(author)
             f.write(
@@ -375,55 +360,48 @@
                     info["date_last"],
                     info["timedelta"],
                     len(info["active_days"]),
                     info["place_by_commits"],
                 )
             )
         f.write("</table>")
-
         allauthors = data.getAuthors()
         if len(allauthors) > conf["max_authors"]:
             rest = allauthors[conf["max_authors"] :]
             f.write(
                 '<p class="moreauthors">These didn\'t make it to the top: %s</p>'
                 % ", ".join(rest)
             )
-
         f.write(html_header(2, "Cumulated Added Lines of Code per Author"))
         f.write(
             '<img src="lines_of_code_by_author.png" alt="Lines of code per Author">'
         )
         if len(allauthors) > conf["max_authors"]:
             f.write(
                 '<p class="moreauthors">Only top %d authors shown</p>'
                 % conf["max_authors"]
             )
-
         f.write(html_header(2, "Commits per Author"))
         f.write('<img src="commits_by_author.png" alt="Commits per Author">')
         if len(allauthors) > conf["max_authors"]:
             f.write(
                 '<p class="moreauthors">Only top %d authors shown</p>'
                 % conf["max_authors"]
             )
-
         fgl = open(path + "/lines_of_code_by_author.dat", "w")
         fgc = open(path + "/commits_by_author.dat", "w")
-
         lines_by_authors = {}  # cumulated added lines by
         # author. to save memory,
         # changes_by_date_by_author[stamp][author] is defined
         # only at points where author commits.
         # lines_by_authors allows us to generate all the
         # points in the .dat file.
-
         # Don't rely on getAuthors to give the same order each
         # time. Be robust and keep the list in a variable.
         commits_by_authors = {}  # cumulated added lines by
-
         self.authors_to_plot = data.getAuthors(conf["max_authors"])
         for author in self.authors_to_plot:
             lines_by_authors[author] = 0
             commits_by_authors[author] = 0
         for stamp in sorted(data.changes_by_date_by_author.keys()):
             fgl.write("%d" % stamp)
             fgc.write("%d" % stamp)
@@ -437,15 +415,14 @@
                     ]["commits"]
                 fgl.write(" %d" % lines_by_authors[author])
                 fgc.write(" %d" % commits_by_authors[author])
             fgl.write("\n")
             fgc.write("\n")
         fgl.close()
         fgc.close()
-
         # Authors :: Author of Month
         f.write(html_header(2, "Author of Month"))
         f.write('<table class="sortable" id="aom">')
         f.write(
             '<tr><th>Month</th><th>Author</th><th>Commits (%%)</th><th class="unsortable">Next top %d</th><th>Number of authors</th></tr>'
             % conf["authors_top"]
         )
@@ -464,17 +441,15 @@
                     commits,
                     (100.0 * commits) / data.commits_by_month[yymm],
                     data.commits_by_month[yymm],
                     next,
                     len(authors),
                 )
             )
-
         f.write("</table>")
-
         f.write(html_header(2, "Author of Year"))
         f.write(
             '<table class="sortable" id="aoy"><tr><th>Year</th><th>Author</th><th>Commits (%%)</th><th class="unsortable">Next top %d</th><th>Number of authors</th></tr>'
             % conf["authors_top"]
         )
         for yy in sorted(data.author_of_year.keys(), reverse=True):
             authordict = data.author_of_year[yy]
@@ -492,15 +467,14 @@
                     (100.0 * commits) / data.commits_by_year[yy],
                     data.commits_by_year[yy],
                     next,
                     len(authors),
                 )
             )
         f.write("</table>")
-
         # Domains
         f.write(html_header(2, "Commits by Domains"))
         domains_by_commits = getkeyssortedbyvaluekey(data.domains, "commits")
         domains_by_commits = list(domains_by_commits)
         domains_by_commits.reverse()  # most first
         f.write('<div class="vtable"><table>')
         f.write("<tr><th>Domains</th><th>Total (%)</th></tr>")
@@ -516,61 +490,51 @@
             f.write(
                 "<tr><th>%s</th><td>%d (%.2f%%)</td></tr>"
                 % (domain, info["commits"], (100.0 * info["commits"] / totalcommits))
             )
         f.write("</table></div>")
         f.write('<img src="domains.png" alt="Commits by Domains">')
         fp.close()
-
         f.write("</body></html>")
         f.close()
 
-        ###
-        # Files
+    def create_files_report(self, data, path):
         f = open(path + "/files.html", "w")
         self.printHeader(f)
         f.write("<h1>Files</h1>")
         self.printNav(f)
-
         f.write("<dl>\n")
         f.write("<dt>Total files</dt><dd>%d</dd>" % data.getTotalFiles())
         f.write("<dt>Total lines</dt><dd>%d</dd>" % data.getTotalLOC())
         with contextlib.suppress(ZeroDivisionError):
             f.write(
                 "<dt>Average file size</dt><dd>%.2f bytes</dd>"
                 % (float(data.getTotalSize()) / data.getTotalFiles())
             )
-
         f.write("</dl>\n")
-
         # Files :: File count by date
         f.write(html_header(2, "File count by date"))
-
         # use set to get rid of duplicate/unnecessary entries
         files_by_date = set()
         for stamp in sorted(data.files_by_stamp.keys()):
             files_by_date.add(
                 "%s %d"
                 % (
                     datetime.datetime.fromtimestamp(stamp).strftime("%Y-%m-%d"),
                     data.files_by_stamp[stamp],
                 )
             )
-
         fg = open(path + "/files_by_date.dat", "w")
         for line in sorted(files_by_date):
             fg.write(f"{line}\n")
         # for stamp in sorted(data.files_by_stamp.keys()):
         # 	fg.write('%s %d\n' % (datetime.datetime.fromtimestamp(stamp).strftime('%Y-%m-%d'), data.files_by_stamp[stamp]))
         fg.close()
-
         f.write('<img src="files_by_date.png" alt="Files by Date">')
-
         # f.write('<h2>Average file size by date</h2>')
-
         # Files :: Extensions
         f.write(html_header(2, "Extensions"))
         f.write(
             '<table class="sortable" id="ext"><tr><th>Extension</th><th>Files (%)</th><th>Lines (%)</th><th>Lines/file</th></tr>'
         )
         for ext in sorted(data.extensions.keys()):
             files = data.extensions[ext]["files"]
@@ -587,56 +551,47 @@
                     (100.0 * files) / data.getTotalFiles(),
                     lines,
                     loc_percentage,
                     lines / files,
                 )
             )
         f.write("</table>")
-
         f.write("</body></html>")
         f.close()
 
-        ###
-        # Lines
+    def create_lines_report(self, data, path):
         f = open(path + "/lines.html", "w")
         self.printHeader(f)
         f.write("<h1>Lines</h1>")
         self.printNav(f)
-
         f.write("<dl>\n")
         f.write("<dt>Total lines</dt><dd>%d</dd>" % data.getTotalLOC())
         f.write("</dl>\n")
-
         f.write(html_header(2, "Lines of Code"))
         f.write('<img src="lines_of_code.png" alt="Lines of Code">')
-
         fg = open(path + "/lines_of_code.dat", "w")
         for stamp in sorted(data.changes_by_date.keys()):
             fg.write("%d %d\n" % (stamp, data.changes_by_date[stamp]["lines"]))
         fg.close()
-
         f.write("</body></html>")
         f.close()
 
-        ###
-        # tags.html
+    def create_tags_report(self, data, path):
         f = open(path + "/tags.html", "w")
         self.printHeader(f)
         f.write("<h1>Tags</h1>")
         self.printNav(f)
-
         f.write("<dl>")
         f.write(f"<dt>Total tags</dt><dd>{len(data.tags)}</dd>")
         if len(data.tags) > 0:
             f.write(
                 "<dt>Average commits per tag</dt><dd>%.2f</dd>"
                 % (1.0 * data.getTotalCommits() / len(data.tags))
             )
         f.write("</dl>")
-
         f.write('<table class="tags">')
         f.write("<tr><th>Name</th><th>Date</th><th>Commits</th><th>Authors</th></tr>")
         # sort the tags by date desc
         tags_sorted_by_date_desc = (
             el[1]
             for el in sorted(
                 ((el[1]["date"], el[0]) for el in data.tags.items()), reverse=True
@@ -655,20 +610,17 @@
                     tag,
                     data.tags[tag]["date"],
                     data.tags[tag]["commits"],
                     ", ".join(authorinfo),
                 )
             )
         f.write("</table>")
-
         f.write("</body></html>")
         f.close()
 
-        self.createGraphs(path)
-
     def createGraphs(self, path):
         print("Generating graphs...")
 
         # hour of day
         f = open(path + "/hour_of_day.plot", "w")
         f.write(GNUPLOT_COMMON)
         f.write(
```

### Comparing `gitstats_abilian-1.0.4/src/gitstats/utils.py` & `gitstats_abilian-1.0.5/src/gitstats/utils.py`

 * *Files identical despite different names*

### Comparing `gitstats_abilian-1.0.4/src/gitstats/version.py` & `gitstats_abilian-1.0.5/src/gitstats/version.py`

 * *Files identical despite different names*

### Comparing `gitstats_abilian-1.0.4/PKG-INFO` & `gitstats_abilian-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitstats-abilian
-Version: 1.0.4
+Version: 1.0.5
 Summary: 
 Author: Stefane Fermigier
 Author-email: sf@abilian.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

