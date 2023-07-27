# Comparing `tmp/photos_where-1.9.tar.gz` & `tmp/photos_where-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "photos_where-1.9.tar", last modified: Fri Jul 21 13:28:06 2023, max compression
+gzip compressed data, was "photos_where-2.1.tar", last modified: Thu Jul 27 11:31:06 2023, max compression
```

## Comparing `photos_where-1.9.tar` & `photos_where-2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 visgean    (501) staff       (20)        0 2023-07-21 13:28:06.760998 photos_where-1.9/
--rw-r--r--   0 visgean    (501) staff       (20)     1063 2022-09-28 18:42:28.000000 photos_where-1.9/LICENSE
--rw-r--r--   0 visgean    (501) staff       (20)       66 2023-07-21 13:11:27.000000 photos_where-1.9/MANIFEST.in
--rw-r--r--   0 visgean    (501) staff       (20)     1943 2023-07-21 13:28:06.760854 photos_where-1.9/PKG-INFO
--rw-r--r--   0 visgean    (501) staff       (20)     1253 2023-07-01 21:31:17.000000 photos_where-1.9/README.md
-drwxr-xr-x   0 visgean    (501) staff       (20)        0 2023-07-21 13:28:06.758451 photos_where-1.9/photos_where/
--rw-r--r--   0 visgean    (501) staff       (20)       25 2023-06-30 22:30:00.000000 photos_where-1.9/photos_where/__init__.py
--rw-r--r--   0 visgean    (501) staff       (20)  7852501 2022-01-28 14:20:56.000000 photos_where-1.9/photos_where/cities.csv
--rwxr-xr-x   0 visgean    (501) staff       (20)     2037 2023-06-30 18:47:13.000000 photos_where-1.9/photos_where/main.py
--rw-r--r--   0 visgean    (501) staff       (20)     5152 2023-07-01 22:17:33.000000 photos_where-1.9/photos_where/where.py
-drwxr-xr-x   0 visgean    (501) staff       (20)        0 2023-07-21 13:28:06.760689 photos_where-1.9/photos_where.egg-info/
--rw-r--r--   0 visgean    (501) staff       (20)     1943 2023-07-21 13:28:06.000000 photos_where-1.9/photos_where.egg-info/PKG-INFO
--rw-r--r--   0 visgean    (501) staff       (20)      363 2023-07-21 13:28:06.000000 photos_where-1.9/photos_where.egg-info/SOURCES.txt
--rw-r--r--   0 visgean    (501) staff       (20)        1 2023-07-21 13:28:06.000000 photos_where-1.9/photos_where.egg-info/dependency_links.txt
--rw-r--r--   0 visgean    (501) staff       (20)       57 2023-07-21 13:28:06.000000 photos_where-1.9/photos_where.egg-info/entry_points.txt
--rw-r--r--   0 visgean    (501) staff       (20)       62 2023-07-21 13:28:06.000000 photos_where-1.9/photos_where.egg-info/requires.txt
--rw-r--r--   0 visgean    (501) staff       (20)       13 2023-07-21 13:28:06.000000 photos_where-1.9/photos_where.egg-info/top_level.txt
--rw-r--r--   0 visgean    (501) staff       (20)      464 2023-07-21 13:24:35.000000 photos_where-1.9/pyproject.toml
--rw-r--r--   0 visgean    (501) staff       (20)       38 2023-07-21 13:28:06.761041 photos_where-1.9/setup.cfg
--rw-r--r--   0 visgean    (501) staff       (20)     1102 2023-07-21 13:25:31.000000 photos_where-1.9/setup.py
+drwxr-xr-x   0 visgean    (501) staff       (20)        0 2023-07-27 11:31:06.778133 photos_where-2.1/
+-rw-r--r--   0 visgean    (501) staff       (20)     1063 2022-09-28 18:42:28.000000 photos_where-2.1/LICENSE
+-rw-r--r--   0 visgean    (501) staff       (20)       66 2023-07-21 13:11:27.000000 photos_where-2.1/MANIFEST.in
+-rw-r--r--   0 visgean    (501) staff       (20)     3183 2023-07-27 11:31:06.777960 photos_where-2.1/PKG-INFO
+-rw-r--r--   0 visgean    (501) staff       (20)     2213 2023-07-27 11:29:37.000000 photos_where-2.1/README.md
+drwxr-xr-x   0 visgean    (501) staff       (20)        0 2023-07-27 11:31:06.766571 photos_where-2.1/photos_where/
+-rw-r--r--   0 visgean    (501) staff       (20)       25 2023-06-30 22:30:00.000000 photos_where-2.1/photos_where/__init__.py
+-rw-r--r--   0 visgean    (501) staff       (20)  7852501 2022-01-28 14:20:56.000000 photos_where-2.1/photos_where/cities.csv
+-rwxr-xr-x   0 visgean    (501) staff       (20)     2121 2023-07-27 10:29:51.000000 photos_where-2.1/photos_where/main.py
+-rw-r--r--   0 visgean    (501) staff       (20)     6214 2023-07-27 11:12:43.000000 photos_where-2.1/photos_where/where.py
+-rw-r--r--   0 visgean    (501) staff       (20)  1101913 2023-07-27 10:55:59.000000 photos_where-2.1/photos_where/world.svg
+drwxr-xr-x   0 visgean    (501) staff       (20)        0 2023-07-27 11:31:06.777739 photos_where-2.1/photos_where.egg-info/
+-rw-r--r--   0 visgean    (501) staff       (20)     3183 2023-07-27 11:31:06.000000 photos_where-2.1/photos_where.egg-info/PKG-INFO
+-rw-r--r--   0 visgean    (501) staff       (20)      371 2023-07-27 11:31:06.000000 photos_where-2.1/photos_where.egg-info/SOURCES.txt
+-rw-r--r--   0 visgean    (501) staff       (20)        1 2023-07-27 11:31:06.000000 photos_where-2.1/photos_where.egg-info/dependency_links.txt
+-rw-r--r--   0 visgean    (501) staff       (20)       57 2023-07-27 11:31:06.000000 photos_where-2.1/photos_where.egg-info/entry_points.txt
+-rw-r--r--   0 visgean    (501) staff       (20)       77 2023-07-27 11:31:06.000000 photos_where-2.1/photos_where.egg-info/requires.txt
+-rw-r--r--   0 visgean    (501) staff       (20)       13 2023-07-27 11:31:06.000000 photos_where-2.1/photos_where.egg-info/top_level.txt
+-rw-r--r--   0 visgean    (501) staff       (20)       38 2023-07-27 11:31:06.778177 photos_where-2.1/setup.cfg
+-rw-r--r--   0 visgean    (501) staff       (20)     1151 2023-07-27 11:12:43.000000 photos_where-2.1/setup.py
```

### Comparing `photos_where-1.9/LICENSE` & `photos_where-2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `photos_where-1.9/PKG-INFO` & `photos_where-2.1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,48 +1,68 @@
-Metadata-Version: 2.1
-Name: photos_where
-Version: 1.9
-Summary: Analyze exif data
-Home-page: https://github.com/visgean/where
-Author: Visgean
-Author-email: visgean@gmail.com
-License: MIT
-Description: # Where - day by day location from your photos 
-        
-        This scripts reads EXIF data from your photos and generates CSV file or Pandas dataframe with day by day location in terms of country. 
-        
-        It relies on my package [exif2pandas](https://github.com/Visgean/exif2pandas/). It uses [reverse-geocoder](https://github.com/thampiman/reverse-geocoder) to convert GPS data to country codes. That module uses a csv file with 150k cities and then uses nearest neighbour algorithm to find the position of each gps data point. This sometimes does not work in border regions so if you are seeing bad data the easiest fix is to copy [cities.csv](https://github.com/Visgean/where/blob/main/src/cities.csv) and add your village etc. 
-        
-        In case some of your photos contain bad gps data that show that you have been to countries where you have never been you can use ``ignore_countries`` argument. 
-        
-        
-        ## Jupyter examples:
-        
-        See ``example.ipynb`` for example graphs and data frames exported.
-        
-        ## Install:
-        
-        See PYPI [Python package](https://pypi.org/project/photos-where/). 
-        
-        ```
-        $ pip install photos-where
-        ```
-        
-        ## Use:
-        
-        ```
-        $ photos_where Dropbox/Photos/2020/
-        $ ls where
-        cities-pie.jpg      
-        countries-pie.jpg
-        intervals.csv
-        location-by-day.csv 
-        photos.feather     
-        years.jpg
-        ```
-        
-Keywords: exif sql
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Description-Content-Type: text/markdown
+# Where - day by day location from your photos 
+
+This scripts reads EXIF data from your photos and generates CSV file or Pandas dataframe with day by day location in terms of country. 
+
+It relies on my package [exif2pandas](https://github.com/Visgean/exif2pandas/). It uses [reverse-geocoder](https://github.com/thampiman/reverse-geocoder) to convert GPS data to country codes. That module uses a csv file with 150k cities and then uses nearest neighbour algorithm to find the position of each gps data point. This sometimes does not work in border regions so if you are seeing bad data the easiest fix is to copy [cities.csv](https://github.com/Visgean/where/blob/main/src/cities.csv) and add your village etc. 
+
+In case some of your photos contain bad gps data that show that you have been to countries where you have never been you can use ``ignore_countries`` argument. 
+
+## world map
+
+![image-20230727131720726](assets/image-20230727131720726.png)
+
+Generated world map with colored regions according to how many days you have spent in the country.
+
+## Pie graph with number of days you spent in a country
+
+![image-20230727131816623](assets/image-20230727131816623.png)
+
+## CSV file with your travel list:
+
+``` 
+id,from,to,days,country,country_code
+4,2015-11-07,2015-11-09,1,Scotland,GB
+5,2015-11-09,2015-12-12,32,Praha,CZ
+6,2015-12-12,2015-12-12,0,Budapest,HU
+7,2015-12-12,2015-12-12,0,Praha,CZ
+8,2015-12-12,2015-12-15,2,Budapest,HU
+
+```
+
+note that the country column is usually wrong - this is because the cities.csv is not consisent with administrative boundaries beyond country_code. 
+
+## Year by year histograms
+
+![image-20230727132504796](assets/image-20230727132504796.png)
+
+## Raw dataframes:
+
+Finally there is a raw dataframe with exif data per image file:
+
+![image-20230727132834377](assets/image-20230727132834377.png)
+
+
+
+## Jupyter examples:
+
+See ``example.ipynb`` for example graphs and data frames exported.
+
+## Install:
+
+See PYPI [Python package](https://pypi.org/project/photos-where/). 
+
+```
+$ pip install photos-where
+```
+
+## Use:
+
+```
+$ photos_where Dropbox/Photos/2020/
+$ ls where
+cities-pie.jpg      
+countries-pie.jpg
+intervals.csv
+location-by-day.csv 
+photos.feather     
+years.jpg
+```
```

### Comparing `photos_where-1.9/photos_where/cities.csv` & `photos_where-2.1/photos_where/cities.csv`

 * *Files identical despite different names*

### Comparing `photos_where-1.9/photos_where/main.py` & `photos_where-2.1/photos_where/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     '-o',
     '--output'
     "out", help="Output folder for the csv etc", default='where',
     dest='out'
 )
 
 parser.add_argument(
-    '-i'
+    '-i',
     "--ignore_countries",
     nargs="+",
     help="Country codes to ignore",
     dest='ignore'
 
 )
 
@@ -55,14 +55,16 @@
     if args.feather:
         feather_loc = Path(args.feather).resolve()
 
     ignore_countries = []
     if args.ignore:
         ignore_countries = args.ignore
 
+    print(f'ignoring: {ignore_countries}')
+
     where = Where(
         feather_location=feather_loc,
         pictures_root=picture_dirs,
         processes=5,
         ignore_countries=ignore_countries
     )
 
@@ -78,10 +80,13 @@
     plt.style.use('seaborn-deep')
     fig = plt.figure(figsize=(15, 20))
     ax = fig.gca()
 
     where.day_df['country_code'].hist(by=where.day_df.index.year, ax=ax, rwidth=0.5)
     savefig(out_dir / 'years.jpg')
 
+    where.generate_wiki_map(out_dir)
+
+
 
 if __name__ == "__main__":
     main()
```

### Comparing `photos_where-1.9/photos_where.egg-info/PKG-INFO` & `photos_where-2.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,58 @@
 Metadata-Version: 2.1
-Name: photos-where
-Version: 1.9
+Name: photos_where
+Version: 2.1
 Summary: Analyze exif data
 Home-page: https://github.com/visgean/where
 Author: Visgean
 Author-email: visgean@gmail.com
 License: MIT
 Description: # Where - day by day location from your photos 
         
         This scripts reads EXIF data from your photos and generates CSV file or Pandas dataframe with day by day location in terms of country. 
         
         It relies on my package [exif2pandas](https://github.com/Visgean/exif2pandas/). It uses [reverse-geocoder](https://github.com/thampiman/reverse-geocoder) to convert GPS data to country codes. That module uses a csv file with 150k cities and then uses nearest neighbour algorithm to find the position of each gps data point. This sometimes does not work in border regions so if you are seeing bad data the easiest fix is to copy [cities.csv](https://github.com/Visgean/where/blob/main/src/cities.csv) and add your village etc. 
         
         In case some of your photos contain bad gps data that show that you have been to countries where you have never been you can use ``ignore_countries`` argument. 
         
+        ## world map
+        
+        ![image-20230727131720726](assets/image-20230727131720726.png)
+        
+        Generated world map with colored regions according to how many days you have spent in the country.
+        
+        ## Pie graph with number of days you spent in a country
+        
+        ![image-20230727131816623](assets/image-20230727131816623.png)
+        
+        ## CSV file with your travel list:
+        
+        ``` 
+        id,from,to,days,country,country_code
+        4,2015-11-07,2015-11-09,1,Scotland,GB
+        5,2015-11-09,2015-12-12,32,Praha,CZ
+        6,2015-12-12,2015-12-12,0,Budapest,HU
+        7,2015-12-12,2015-12-12,0,Praha,CZ
+        8,2015-12-12,2015-12-15,2,Budapest,HU
+        
+        ```
+        
+        note that the country column is usually wrong - this is because the cities.csv is not consisent with administrative boundaries beyond country_code. 
+        
+        ## Year by year histograms
+        
+        ![image-20230727132504796](assets/image-20230727132504796.png)
+        
+        ## Raw dataframes:
+        
+        Finally there is a raw dataframe with exif data per image file:
+        
+        ![image-20230727132834377](assets/image-20230727132834377.png)
+        
+        
         
         ## Jupyter examples:
         
         See ``example.ipynb`` for example graphs and data frames exported.
         
         ## Install:
```

### Comparing `photos_where-1.9/setup.py` & `photos_where-2.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,37 +8,39 @@
     from distutils.core import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="photos_where",
-    version="1.9",
+    version="2.1",
     description="Analyze exif data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Visgean",
     author_email="visgean@gmail.com",
     url="https://github.com/visgean/where",
     packages=[
         "photos_where",
     ],
     package_dir={"photos_where": "photos_where"},
     package_data={
-        'photos_where': ['cities.csv'],
+        'photos_where': ['cities.csv', 'world.svg'],
     },
     license="MIT",
     keywords="exif sql",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
     ],
     install_requires=[
         "exif2pandas",
         "pandas",
         "matplotlib",
         "reverse-geocoder==1.5.1",
         "pyarrow",
+        "Jinja2",
+        "seaborn"
     ],
     entry_points={"console_scripts": ["photos_where = photos_where.main:main"]},
 )
```

