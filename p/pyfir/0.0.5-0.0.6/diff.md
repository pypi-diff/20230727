# Comparing `tmp/pyfir-0.0.5.tar.gz` & `tmp/pyfir-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfir-0.0.5.tar", last modified: Sat Oct  2 17:21:00 2021, max compression
+gzip compressed data, was "pyfir-0.0.6.tar", last modified: Thu Jul 27 15:18:27 2023, max compression
```

## Comparing `pyfir-0.0.5.tar` & `pyfir-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 claudjo   (1000) claudjo   (1000)        0 2021-10-02 17:21:00.469939 pyfir-0.0.5/
--rw-rw-r--   0 claudjo   (1000) claudjo   (1000)     2503 2021-10-02 17:21:00.469939 pyfir-0.0.5/PKG-INFO
--rw-rw-r--   0 claudjo   (1000) claudjo   (1000)     1552 2021-10-02 17:19:28.000000 pyfir-0.0.5/README.md
-drwxrwxr-x   0 claudjo   (1000) claudjo   (1000)        0 2021-10-02 17:21:00.469939 pyfir-0.0.5/fir/
--rw-rw-r--   0 claudjo   (1000) claudjo   (1000)        0 2021-10-02 16:52:36.000000 pyfir-0.0.5/fir/__init__.py
--rw-rw-r--   0 claudjo   (1000) claudjo   (1000)     2901 2021-10-02 16:52:36.000000 pyfir-0.0.5/fir/http.py
--rw-rw-r--   0 claudjo   (1000) claudjo   (1000)     2672 2021-10-02 16:52:36.000000 pyfir-0.0.5/fir/wsgi.py
-drwxrwxr-x   0 claudjo   (1000) claudjo   (1000)        0 2021-10-02 17:21:00.469939 pyfir-0.0.5/pyfir.egg-info/
--rw-rw-r--   0 claudjo   (1000) claudjo   (1000)     2503 2021-10-02 17:21:00.000000 pyfir-0.0.5/pyfir.egg-info/PKG-INFO
--rw-rw-r--   0 claudjo   (1000) claudjo   (1000)      174 2021-10-02 17:21:00.000000 pyfir-0.0.5/pyfir.egg-info/SOURCES.txt
--rw-rw-r--   0 claudjo   (1000) claudjo   (1000)        1 2021-10-02 17:21:00.000000 pyfir-0.0.5/pyfir.egg-info/dependency_links.txt
--rw-rw-r--   0 claudjo   (1000) claudjo   (1000)        4 2021-10-02 17:21:00.000000 pyfir-0.0.5/pyfir.egg-info/top_level.txt
--rw-rw-r--   0 claudjo   (1000) claudjo   (1000)       38 2021-10-02 17:21:00.469939 pyfir-0.0.5/setup.cfg
--rw-rw-r--   0 claudjo   (1000) claudjo   (1000)      724 2021-10-02 16:52:36.000000 pyfir-0.0.5/setup.py
+drwxrwxr-x   0 claudjo   (1000) claudjo   (1000)        0 2023-07-27 15:18:27.924711 pyfir-0.0.6/
+-rw-rw-r--   0 claudjo   (1000) claudjo   (1000)     1072 2023-07-27 15:03:16.000000 pyfir-0.0.6/LICENSE
+-rw-rw-r--   0 claudjo   (1000) claudjo   (1000)     1866 2023-07-27 15:18:27.924711 pyfir-0.0.6/PKG-INFO
+-rw-rw-r--   0 claudjo   (1000) claudjo   (1000)     1552 2023-07-27 15:03:16.000000 pyfir-0.0.6/README.md
+drwxrwxr-x   0 claudjo   (1000) claudjo   (1000)        0 2023-07-27 15:18:27.920711 pyfir-0.0.6/fir/
+-rw-rw-r--   0 claudjo   (1000) claudjo   (1000)        0 2023-07-27 15:03:16.000000 pyfir-0.0.6/fir/__init__.py
+-rw-rw-r--   0 claudjo   (1000) claudjo   (1000)     2901 2023-07-27 15:03:16.000000 pyfir-0.0.6/fir/http.py
+-rw-rw-r--   0 claudjo   (1000) claudjo   (1000)     2677 2023-07-27 15:05:48.000000 pyfir-0.0.6/fir/wsgi.py
+drwxrwxr-x   0 claudjo   (1000) claudjo   (1000)        0 2023-07-27 15:18:27.924711 pyfir-0.0.6/pyfir.egg-info/
+-rw-rw-r--   0 claudjo   (1000) claudjo   (1000)     1866 2023-07-27 15:18:27.000000 pyfir-0.0.6/pyfir.egg-info/PKG-INFO
+-rw-rw-r--   0 claudjo   (1000) claudjo   (1000)      182 2023-07-27 15:18:27.000000 pyfir-0.0.6/pyfir.egg-info/SOURCES.txt
+-rw-rw-r--   0 claudjo   (1000) claudjo   (1000)        1 2023-07-27 15:18:27.000000 pyfir-0.0.6/pyfir.egg-info/dependency_links.txt
+-rw-rw-r--   0 claudjo   (1000) claudjo   (1000)        4 2023-07-27 15:18:27.000000 pyfir-0.0.6/pyfir.egg-info/top_level.txt
+-rw-rw-r--   0 claudjo   (1000) claudjo   (1000)       38 2023-07-27 15:18:27.924711 pyfir-0.0.6/setup.cfg
+-rw-rw-r--   0 claudjo   (1000) claudjo   (1000)      724 2023-07-27 15:11:27.000000 pyfir-0.0.6/setup.py
```

### Comparing `pyfir-0.0.5/README.md` & `pyfir-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pyfir-0.0.5/fir/http.py` & `pyfir-0.0.6/fir/http.py`

 * *Files identical despite different names*

### Comparing `pyfir-0.0.5/fir/wsgi.py` & `pyfir-0.0.6/fir/wsgi.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 		"PATH_INFO": request.path,
 		"RAW_URI": request.uri,
 		"QUERY_STRING": request.query,
 		"SERVER_NAME": server_name,
 	}
 
 	if body != b'':
-		environ["CONTENT_LENGTH"] = len(body)
+		environ["CONTENT_LENGTH"] = str(len(body))
 		if request.headers.get("content-type") is not None:
 			environ["CONTENT_TYPE"] = request.headers.get("content-type", "*/*")
 
 	for header_name, value in request.headers.items():
 		key = "HTTP_{}".format(header_name.upper().replace("-", "_"))
 		environ[key] = value
```

### Comparing `pyfir-0.0.5/setup.py` & `pyfir-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 NAME = "pyfir"
-VERSION = "0.0.5"
+VERSION = "0.0.6"
 
 REQUIRES = []
 
 
 setup(
     name=NAME,
     version=VERSION,
```

