# Comparing `tmp/productmd-1.8.tar.bz2` & `tmp/productmd-1.9.tar.bz2`

## Comparing `productmd-1.8.tar` & `productmd-1.9.tar`

### file list

```diff
@@ -1,198 +1,198 @@
-drwxrwxr-x   0 lsedlar   (1000) lsedlar   (1000)        0 2017-10-30 06:31:20.000000 productmd-1.8/
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      293 2017-01-05 07:03:39.000000 productmd-1.8/MANIFEST.in
-drwxrwxr-x   0 lsedlar   (1000) lsedlar   (1000)        0 2017-10-30 06:31:20.000000 productmd-1.8/productmd.egg-info/
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       10 2017-10-30 06:31:20.000000 productmd-1.8/productmd.egg-info/top_level.txt
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)        1 2017-10-30 06:31:20.000000 productmd-1.8/productmd.egg-info/dependency_links.txt
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)        4 2017-10-30 06:31:20.000000 productmd-1.8/productmd.egg-info/requires.txt
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     6304 2017-10-30 06:31:20.000000 productmd-1.8/productmd.egg-info/SOURCES.txt
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      285 2017-10-30 06:31:20.000000 productmd-1.8/productmd.egg-info/PKG-INFO
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       63 2017-10-30 06:31:20.000000 productmd-1.8/setup.cfg
-drwxrwxr-x   0 lsedlar   (1000) lsedlar   (1000)        0 2017-10-30 06:31:20.000000 productmd-1.8/doc/
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     9191 2016-08-29 12:03:59.000000 productmd-1.8/doc/conf.py
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      937 2016-04-13 14:22:45.000000 productmd-1.8/doc/common.rst
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      654 2015-05-05 08:37:42.000000 productmd-1.8/doc/discinfo-1.0.rst
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     7378 2015-05-05 08:37:42.000000 productmd-1.8/doc/treeinfo-1.0.rst
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     2155 2016-09-29 06:40:46.000000 productmd-1.8/doc/composeinfo-1.1.rst
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      264 2016-01-26 08:47:58.000000 productmd-1.8/doc/compose.rst
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      292 2015-05-05 08:37:42.000000 productmd-1.8/doc/images.rst
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     6411 2016-04-13 14:22:45.000000 productmd-1.8/doc/rpms-1.0.rst
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     2924 2017-03-27 07:00:17.000000 productmd-1.8/doc/images-1.1.rst
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1716 2016-09-29 06:40:46.000000 productmd-1.8/doc/composeinfo-1.0.rst
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     5576 2015-05-05 08:37:42.000000 productmd-1.8/doc/Makefile
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      254 2015-05-05 08:37:42.000000 productmd-1.8/doc/discinfo.rst
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     3972 2016-02-19 08:28:55.000000 productmd-1.8/doc/terminology.rst
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     2231 2016-08-29 12:03:59.000000 productmd-1.8/doc/images-1.0.rst
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      185 2015-05-05 08:37:42.000000 productmd-1.8/doc/rpms.rst
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      965 2015-05-05 08:37:42.000000 productmd-1.8/doc/composeinfo.rst
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      720 2016-08-29 12:03:59.000000 productmd-1.8/doc/index.rst
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      607 2015-05-05 08:37:42.000000 productmd-1.8/doc/treeinfo.rst
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     6621 2016-08-29 12:03:59.000000 productmd-1.8/doc/rpms-1.1.rst
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     7880 2016-08-29 12:03:59.000000 productmd-1.8/doc/treeinfo-1.1.rst
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1488 2016-11-23 07:41:29.000000 productmd-1.8/Makefile
-drwxrwxr-x   0 lsedlar   (1000) lsedlar   (1000)        0 2017-10-30 06:31:20.000000 productmd-1.8/productmd/
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1005 2017-01-02 11:57:41.000000 productmd-1.8/productmd/__init__.py
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)    39356 2016-11-15 15:04:26.000000 productmd-1.8/productmd/treeinfo.py
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     3580 2016-08-29 12:03:59.000000 productmd-1.8/productmd/discinfo.py
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)    15616 2017-10-30 06:30:37.000000 productmd-1.8/productmd/common.py
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     4137 2017-10-04 06:09:51.000000 productmd-1.8/productmd/compose.py
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)    29455 2017-10-03 08:39:40.000000 productmd-1.8/productmd/composeinfo.py
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)    12012 2017-10-03 09:07:19.000000 productmd-1.8/productmd/images.py
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     5637 2016-08-29 12:03:59.000000 productmd-1.8/productmd/rpms.py
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       43 2015-05-05 08:37:42.000000 productmd-1.8/AUTHORS
--rwxrwxr-x   0 lsedlar   (1000) lsedlar   (1000)      880 2017-10-30 06:30:37.000000 productmd-1.8/setup.py
-drwxrwxr-x   0 lsedlar   (1000) lsedlar   (1000)        0 2017-10-30 06:31:20.000000 productmd-1.8/tests/
--rwxrwxr-x   0 lsedlar   (1000) lsedlar   (1000)     3844 2016-08-29 12:03:59.000000 productmd-1.8/tests/test_rpms.py
--rwxrwxr-x   0 lsedlar   (1000) lsedlar   (1000)     3361 2017-02-03 07:50:00.000000 productmd-1.8/tests/test_compose.py
-drwxrwxr-x   0 lsedlar   (1000) lsedlar   (1000)        0 2017-10-30 06:31:20.000000 productmd-1.8/tests/discinfo/
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       35 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-16-Fedora.x86_64
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       33 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-16-Fedora.i386
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       88 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-4.x86_64
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      137 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-8-Everything.i386
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       35 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-19-Fedora.x86_64
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       42 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-21-Server.x86_64
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       37 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-14-Fedora.i386
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      115 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-8-Fedora.x86_64
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       35 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-9-Fedora.ppc
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       47 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-21-Alpha-Cloud.x86_64
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       33 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-16-Everything.i386
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       83 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-5.ppc
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       35 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-20-Fedora.armhfp
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       39 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-11-Fedora.x86_64
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       41 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-21-Cloud.x86_64
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       36 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-9-Fedora.i386
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      111 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-8-Fedora.i386
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       45 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-21-Alpha-Cloud.i386
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       53 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-21-Alpha-Workstation.armhfp
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      135 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-8-Everything.ppc
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       39 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-13-Fedora.x86_64
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       33 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-17-Fedora.i386
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      111 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-7-Everything.i386
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       36 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-10-Fedora.ppc
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       53 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-21-Alpha-Workstation.x86_64
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      109 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-8-Fedora.ppc
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       85 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-4.ppc
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       41 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-21-Cloud.armhfp
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       40 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-21-Server.i386
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       35 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-20-Fedora.x86_64
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       35 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-17-Fedora.x86_64
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       36 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-11-Fedora.ppc
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       35 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-16-Everything.x86_64
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       86 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-2.x86_64
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       35 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-18-Fedora.x86_64
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       90 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-6.x86_64
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       39 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-14-Fedora.x86_64
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       86 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-4.i386
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       48 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-11-Everything.x86_64
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       37 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-11-Fedora.i386
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       77 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-1.x86_64
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       87 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-6.ppc
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       46 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-21-Alpha-Server.i386
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       35 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-15-Fedora.x86_64
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       46 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-11-Everything.i386
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      105 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-7-Everything.ppc
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       42 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-21-Server.armhfp
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       39 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-10-Fedora.x86_64
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       47 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-21-Alpha-Cloud.armhfp
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      141 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-8-Everything.x86_64
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       45 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-11-Everything.ppc
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       36 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-12-Fedora.ppc
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       84 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-2.i386
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       35 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-18-Everything.x86_64
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      115 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-7-Everything.x86_64
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       39 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-12-Fedora.x86_64
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       48 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-21-Alpha-Server.armhfp
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       37 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-12-Fedora.i386
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      105 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-7-Fedora.ppc
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       86 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-3.x86_64
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       37 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-13-Fedora.i386
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       86 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-5.x86_64
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       33 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-15-Fedora.i386
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       33 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-18-Everything.i386
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      107 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-7-Fedora.i386
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       37 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-10-Fedora.i386
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       33 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-19-Fedora.i386
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       51 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-21-Alpha-Workstation.i386
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       48 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-21-Alpha-Server.x86_64
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       84 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-3.i386
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       39 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-21-Cloud.i386
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       86 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-6.i386
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       38 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-9-Fedora.x86_64
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       84 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-5.i386
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       33 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-18-Fedora.i386
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       33 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-20-Fedora.i386
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      111 2015-05-05 08:37:42.000000 productmd-1.8/tests/discinfo/fedora-7-Fedora.x86_64
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)        0 2015-05-05 08:37:42.000000 productmd-1.8/tests/__init__.py
--rwxrwxr-x   0 lsedlar   (1000) lsedlar   (1000)     3318 2016-08-29 12:03:59.000000 productmd-1.8/tests/test_common.py
--rwxrwxr-x   0 lsedlar   (1000) lsedlar   (1000)     4440 2016-08-29 12:03:59.000000 productmd-1.8/tests/test_discinfo.py
--rwxrwxr-x   0 lsedlar   (1000) lsedlar   (1000)     9150 2017-01-06 09:03:01.000000 productmd-1.8/tests/test_treeinfo.py
-drwxrwxr-x   0 lsedlar   (1000) lsedlar   (1000)        0 2017-10-30 06:31:20.000000 productmd-1.8/tests/images/
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     2967 2016-08-29 12:03:59.000000 productmd-1.8/tests/images/f23.json
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     3395 2016-08-29 12:03:59.000000 productmd-1.8/tests/images/src_move_before.json
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     2214 2016-08-29 12:03:59.000000 productmd-1.8/tests/images/f20.json
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     4325 2016-08-29 12:03:59.000000 productmd-1.8/tests/images/src_move_after.json
--rwxrwxr-x   0 lsedlar   (1000) lsedlar   (1000)    13027 2017-04-04 07:47:33.000000 productmd-1.8/tests/test_images.py
--rwxrwxr-x   0 lsedlar   (1000) lsedlar   (1000)     2271 2016-08-29 12:03:59.000000 productmd-1.8/tests/test_header.py
--rwxrwxr-x   0 lsedlar   (1000) lsedlar   (1000)     9605 2017-03-27 07:00:17.000000 productmd-1.8/tests/test_composeinfo.py
-drwxrwxr-x   0 lsedlar   (1000) lsedlar   (1000)        0 2017-10-30 06:31:20.000000 productmd-1.8/tests/treeinfo/
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      883 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-16-Fedora.x86_64
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      906 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-16-Fedora.i386
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      434 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-8-Everything.i386
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1117 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-19-Fedora.x86_64
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1224 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-21-Server.x86_64
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1253 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-14-Fedora.i386
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      434 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-8-Fedora.x86_64
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      428 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-9-Fedora.ppc
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1140 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-21-Alpha-Cloud.x86_64
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      900 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-16-Everything.i386
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)    13568 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-20-Fedora.armhfp
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1228 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-11-Fedora.x86_64
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1221 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-21-Cloud.x86_64
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      386 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-9-Fedora.i386
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      430 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-8-Fedora.i386
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1272 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-21-Alpha-Cloud.i386
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)    27048 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-21-Alpha-Workstation.armhfp
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      440 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-8-Everything.ppc
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1228 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-13-Fedora.x86_64
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      948 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-17-Fedora.i386
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      362 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-7-Everything.i386
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1501 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-10-Fedora.ppc
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1158 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-21-Alpha-Workstation.x86_64
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      436 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-8-Fedora.ppc
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)    31238 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-21-Cloud.armhfp
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1356 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-21-Server.i386
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1117 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-20-Fedora.x86_64
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      925 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-17-Fedora.x86_64
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1917 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-11-Fedora.ppc
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      877 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-16-Everything.x86_64
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1117 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-18-Fedora.x86_64
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1044 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-14-Fedora.x86_64
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1437 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-11-Fedora.i386
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1275 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-21-Alpha-Server.i386
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      883 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-15-Fedora.x86_64
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      147 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-7-Everything.ppc
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)    31241 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-21-Server.armhfp
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1002 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-10-Fedora.x86_64
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)    27029 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-21-Alpha-Cloud.armhfp
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      438 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-8-Everything.x86_64
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1917 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-12-Fedora.ppc
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1111 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-18-Everything.x86_64
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      366 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-7-Everything.x86_64
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1228 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-12-Fedora.x86_64
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)    27033 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-21-Alpha-Server.armhfp
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1437 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-12-Fedora.i386
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      364 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-7-Fedora.ppc
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1437 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-13-Fedora.i386
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      906 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-15-Fedora.i386
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1243 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-18-Everything.i386
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      358 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-7-Fedora.i386
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1159 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-10-Fedora.i386
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1249 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-19-Fedora.i386
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1290 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-21-Alpha-Workstation.i386
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1143 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-21-Alpha-Server.x86_64
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1353 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-21-Cloud.i386
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      390 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-9-Fedora.x86_64
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1249 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-18-Fedora.i386
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1249 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-20-Fedora.i386
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      362 2015-05-05 08:37:42.000000 productmd-1.8/tests/treeinfo/fedora-7-Fedora.x86_64
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      285 2017-10-30 06:31:20.000000 productmd-1.8/PKG-INFO
--rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)    26444 2015-05-05 08:37:42.000000 productmd-1.8/LICENSE
+drwxrwxr-x   0 lsedlar   (1000) lsedlar   (1000)        0 2017-10-30 06:31:57.000000 productmd-1.9/
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      293 2017-01-05 07:03:39.000000 productmd-1.9/MANIFEST.in
+drwxrwxr-x   0 lsedlar   (1000) lsedlar   (1000)        0 2017-10-30 06:31:57.000000 productmd-1.9/productmd.egg-info/
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       10 2017-10-30 06:31:57.000000 productmd-1.9/productmd.egg-info/top_level.txt
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)        1 2017-10-30 06:31:57.000000 productmd-1.9/productmd.egg-info/dependency_links.txt
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)        4 2017-10-30 06:31:57.000000 productmd-1.9/productmd.egg-info/requires.txt
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     6304 2017-10-30 06:31:57.000000 productmd-1.9/productmd.egg-info/SOURCES.txt
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      285 2017-10-30 06:31:57.000000 productmd-1.9/productmd.egg-info/PKG-INFO
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       63 2017-10-30 06:31:57.000000 productmd-1.9/setup.cfg
+drwxrwxr-x   0 lsedlar   (1000) lsedlar   (1000)        0 2017-10-30 06:31:57.000000 productmd-1.9/doc/
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     9191 2016-08-29 12:03:59.000000 productmd-1.9/doc/conf.py
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      937 2016-04-13 14:22:45.000000 productmd-1.9/doc/common.rst
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      654 2015-05-05 08:37:42.000000 productmd-1.9/doc/discinfo-1.0.rst
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     7378 2015-05-05 08:37:42.000000 productmd-1.9/doc/treeinfo-1.0.rst
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     2155 2016-09-29 06:40:46.000000 productmd-1.9/doc/composeinfo-1.1.rst
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      264 2016-01-26 08:47:58.000000 productmd-1.9/doc/compose.rst
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      292 2015-05-05 08:37:42.000000 productmd-1.9/doc/images.rst
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     6411 2016-04-13 14:22:45.000000 productmd-1.9/doc/rpms-1.0.rst
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     2924 2017-03-27 07:00:17.000000 productmd-1.9/doc/images-1.1.rst
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1716 2016-09-29 06:40:46.000000 productmd-1.9/doc/composeinfo-1.0.rst
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     5576 2015-05-05 08:37:42.000000 productmd-1.9/doc/Makefile
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      254 2015-05-05 08:37:42.000000 productmd-1.9/doc/discinfo.rst
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     3972 2016-02-19 08:28:55.000000 productmd-1.9/doc/terminology.rst
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     2231 2016-08-29 12:03:59.000000 productmd-1.9/doc/images-1.0.rst
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      185 2015-05-05 08:37:42.000000 productmd-1.9/doc/rpms.rst
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      965 2015-05-05 08:37:42.000000 productmd-1.9/doc/composeinfo.rst
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      720 2016-08-29 12:03:59.000000 productmd-1.9/doc/index.rst
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      607 2015-05-05 08:37:42.000000 productmd-1.9/doc/treeinfo.rst
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     6621 2016-08-29 12:03:59.000000 productmd-1.9/doc/rpms-1.1.rst
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     7880 2016-08-29 12:03:59.000000 productmd-1.9/doc/treeinfo-1.1.rst
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1488 2016-11-23 07:41:29.000000 productmd-1.9/Makefile
+drwxrwxr-x   0 lsedlar   (1000) lsedlar   (1000)        0 2017-10-30 06:31:57.000000 productmd-1.9/productmd/
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1005 2017-01-02 11:57:41.000000 productmd-1.9/productmd/__init__.py
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)    39356 2016-11-15 15:04:26.000000 productmd-1.9/productmd/treeinfo.py
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     3580 2016-08-29 12:03:59.000000 productmd-1.9/productmd/discinfo.py
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)    15639 2017-10-30 06:31:51.000000 productmd-1.9/productmd/common.py
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     4137 2017-10-04 06:09:51.000000 productmd-1.9/productmd/compose.py
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)    29455 2017-10-03 08:39:40.000000 productmd-1.9/productmd/composeinfo.py
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)    12012 2017-10-03 09:07:19.000000 productmd-1.9/productmd/images.py
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     5637 2016-08-29 12:03:59.000000 productmd-1.9/productmd/rpms.py
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       43 2015-05-05 08:37:42.000000 productmd-1.9/AUTHORS
+-rwxrwxr-x   0 lsedlar   (1000) lsedlar   (1000)      880 2017-10-30 06:31:51.000000 productmd-1.9/setup.py
+drwxrwxr-x   0 lsedlar   (1000) lsedlar   (1000)        0 2017-10-30 06:31:57.000000 productmd-1.9/tests/
+-rwxrwxr-x   0 lsedlar   (1000) lsedlar   (1000)     3844 2016-08-29 12:03:59.000000 productmd-1.9/tests/test_rpms.py
+-rwxrwxr-x   0 lsedlar   (1000) lsedlar   (1000)     3361 2017-02-03 07:50:00.000000 productmd-1.9/tests/test_compose.py
+drwxrwxr-x   0 lsedlar   (1000) lsedlar   (1000)        0 2017-10-30 06:31:57.000000 productmd-1.9/tests/discinfo/
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       35 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-16-Fedora.x86_64
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       33 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-16-Fedora.i386
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       88 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-4.x86_64
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      137 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-8-Everything.i386
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       35 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-19-Fedora.x86_64
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       42 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-21-Server.x86_64
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       37 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-14-Fedora.i386
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      115 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-8-Fedora.x86_64
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       35 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-9-Fedora.ppc
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       47 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-21-Alpha-Cloud.x86_64
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       33 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-16-Everything.i386
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       83 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-5.ppc
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       35 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-20-Fedora.armhfp
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       39 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-11-Fedora.x86_64
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       41 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-21-Cloud.x86_64
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       36 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-9-Fedora.i386
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      111 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-8-Fedora.i386
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       45 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-21-Alpha-Cloud.i386
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       53 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-21-Alpha-Workstation.armhfp
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      135 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-8-Everything.ppc
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       39 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-13-Fedora.x86_64
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       33 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-17-Fedora.i386
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      111 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-7-Everything.i386
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       36 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-10-Fedora.ppc
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       53 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-21-Alpha-Workstation.x86_64
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      109 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-8-Fedora.ppc
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       85 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-4.ppc
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       41 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-21-Cloud.armhfp
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       40 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-21-Server.i386
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       35 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-20-Fedora.x86_64
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       35 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-17-Fedora.x86_64
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       36 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-11-Fedora.ppc
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       35 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-16-Everything.x86_64
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       86 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-2.x86_64
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       35 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-18-Fedora.x86_64
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       90 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-6.x86_64
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       39 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-14-Fedora.x86_64
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       86 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-4.i386
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       48 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-11-Everything.x86_64
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       37 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-11-Fedora.i386
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       77 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-1.x86_64
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       87 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-6.ppc
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       46 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-21-Alpha-Server.i386
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       35 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-15-Fedora.x86_64
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       46 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-11-Everything.i386
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      105 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-7-Everything.ppc
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       42 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-21-Server.armhfp
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       39 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-10-Fedora.x86_64
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       47 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-21-Alpha-Cloud.armhfp
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      141 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-8-Everything.x86_64
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       45 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-11-Everything.ppc
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       36 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-12-Fedora.ppc
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       84 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-2.i386
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       35 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-18-Everything.x86_64
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      115 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-7-Everything.x86_64
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       39 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-12-Fedora.x86_64
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       48 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-21-Alpha-Server.armhfp
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       37 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-12-Fedora.i386
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      105 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-7-Fedora.ppc
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       86 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-3.x86_64
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       37 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-13-Fedora.i386
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       86 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-5.x86_64
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       33 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-15-Fedora.i386
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       33 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-18-Everything.i386
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      107 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-7-Fedora.i386
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       37 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-10-Fedora.i386
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       33 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-19-Fedora.i386
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       51 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-21-Alpha-Workstation.i386
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       48 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-21-Alpha-Server.x86_64
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       84 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-3.i386
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       39 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-21-Cloud.i386
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       86 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-6.i386
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       38 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-9-Fedora.x86_64
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       84 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-5.i386
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       33 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-18-Fedora.i386
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)       33 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-20-Fedora.i386
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      111 2015-05-05 08:37:42.000000 productmd-1.9/tests/discinfo/fedora-7-Fedora.x86_64
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)        0 2015-05-05 08:37:42.000000 productmd-1.9/tests/__init__.py
+-rwxrwxr-x   0 lsedlar   (1000) lsedlar   (1000)     3318 2016-08-29 12:03:59.000000 productmd-1.9/tests/test_common.py
+-rwxrwxr-x   0 lsedlar   (1000) lsedlar   (1000)     4440 2016-08-29 12:03:59.000000 productmd-1.9/tests/test_discinfo.py
+-rwxrwxr-x   0 lsedlar   (1000) lsedlar   (1000)     9150 2017-01-06 09:03:01.000000 productmd-1.9/tests/test_treeinfo.py
+drwxrwxr-x   0 lsedlar   (1000) lsedlar   (1000)        0 2017-10-30 06:31:57.000000 productmd-1.9/tests/images/
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     2967 2016-08-29 12:03:59.000000 productmd-1.9/tests/images/f23.json
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     3395 2016-08-29 12:03:59.000000 productmd-1.9/tests/images/src_move_before.json
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     2214 2016-08-29 12:03:59.000000 productmd-1.9/tests/images/f20.json
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     4325 2016-08-29 12:03:59.000000 productmd-1.9/tests/images/src_move_after.json
+-rwxrwxr-x   0 lsedlar   (1000) lsedlar   (1000)    13027 2017-04-04 07:47:33.000000 productmd-1.9/tests/test_images.py
+-rwxrwxr-x   0 lsedlar   (1000) lsedlar   (1000)     2271 2016-08-29 12:03:59.000000 productmd-1.9/tests/test_header.py
+-rwxrwxr-x   0 lsedlar   (1000) lsedlar   (1000)     9605 2017-03-27 07:00:17.000000 productmd-1.9/tests/test_composeinfo.py
+drwxrwxr-x   0 lsedlar   (1000) lsedlar   (1000)        0 2017-10-30 06:31:57.000000 productmd-1.9/tests/treeinfo/
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      883 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-16-Fedora.x86_64
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      906 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-16-Fedora.i386
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      434 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-8-Everything.i386
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1117 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-19-Fedora.x86_64
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1224 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-21-Server.x86_64
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1253 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-14-Fedora.i386
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      434 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-8-Fedora.x86_64
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      428 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-9-Fedora.ppc
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1140 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-21-Alpha-Cloud.x86_64
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      900 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-16-Everything.i386
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)    13568 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-20-Fedora.armhfp
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1228 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-11-Fedora.x86_64
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1221 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-21-Cloud.x86_64
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      386 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-9-Fedora.i386
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      430 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-8-Fedora.i386
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1272 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-21-Alpha-Cloud.i386
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)    27048 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-21-Alpha-Workstation.armhfp
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      440 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-8-Everything.ppc
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1228 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-13-Fedora.x86_64
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      948 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-17-Fedora.i386
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      362 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-7-Everything.i386
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1501 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-10-Fedora.ppc
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1158 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-21-Alpha-Workstation.x86_64
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      436 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-8-Fedora.ppc
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)    31238 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-21-Cloud.armhfp
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1356 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-21-Server.i386
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1117 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-20-Fedora.x86_64
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      925 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-17-Fedora.x86_64
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1917 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-11-Fedora.ppc
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      877 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-16-Everything.x86_64
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1117 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-18-Fedora.x86_64
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1044 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-14-Fedora.x86_64
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1437 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-11-Fedora.i386
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1275 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-21-Alpha-Server.i386
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      883 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-15-Fedora.x86_64
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      147 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-7-Everything.ppc
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)    31241 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-21-Server.armhfp
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1002 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-10-Fedora.x86_64
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)    27029 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-21-Alpha-Cloud.armhfp
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      438 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-8-Everything.x86_64
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1917 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-12-Fedora.ppc
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1111 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-18-Everything.x86_64
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      366 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-7-Everything.x86_64
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1228 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-12-Fedora.x86_64
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)    27033 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-21-Alpha-Server.armhfp
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1437 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-12-Fedora.i386
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      364 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-7-Fedora.ppc
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1437 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-13-Fedora.i386
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      906 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-15-Fedora.i386
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1243 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-18-Everything.i386
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      358 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-7-Fedora.i386
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1159 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-10-Fedora.i386
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1249 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-19-Fedora.i386
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1290 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-21-Alpha-Workstation.i386
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1143 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-21-Alpha-Server.x86_64
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1353 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-21-Cloud.i386
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      390 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-9-Fedora.x86_64
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1249 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-18-Fedora.i386
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)     1249 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-20-Fedora.i386
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      362 2015-05-05 08:37:42.000000 productmd-1.9/tests/treeinfo/fedora-7-Fedora.x86_64
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)      285 2017-10-30 06:31:57.000000 productmd-1.9/PKG-INFO
+-rw-rw-r--   0 lsedlar   (1000) lsedlar   (1000)    26444 2015-05-05 08:37:42.000000 productmd-1.9/LICENSE
```

### Comparing `productmd-1.8/productmd.egg-info/SOURCES.txt` & `productmd-1.9/productmd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `productmd-1.8/doc/conf.py` & `productmd-1.9/doc/conf.py`

 * *Files identical despite different names*

### Comparing `productmd-1.8/doc/common.rst` & `productmd-1.9/doc/common.rst`

 * *Files identical despite different names*

### Comparing `productmd-1.8/doc/discinfo-1.0.rst` & `productmd-1.9/doc/discinfo-1.0.rst`

 * *Files identical despite different names*

### Comparing `productmd-1.8/doc/treeinfo-1.0.rst` & `productmd-1.9/doc/treeinfo-1.0.rst`

 * *Files identical despite different names*

### Comparing `productmd-1.8/doc/composeinfo-1.1.rst` & `productmd-1.9/doc/composeinfo-1.1.rst`

 * *Files identical despite different names*

### Comparing `productmd-1.8/doc/rpms-1.0.rst` & `productmd-1.9/doc/rpms-1.0.rst`

 * *Files identical despite different names*

### Comparing `productmd-1.8/doc/images-1.1.rst` & `productmd-1.9/doc/images-1.1.rst`

 * *Files identical despite different names*

### Comparing `productmd-1.8/doc/composeinfo-1.0.rst` & `productmd-1.9/doc/composeinfo-1.0.rst`

 * *Files identical despite different names*

### Comparing `productmd-1.8/doc/Makefile` & `productmd-1.9/doc/Makefile`

 * *Files identical despite different names*

### Comparing `productmd-1.8/doc/terminology.rst` & `productmd-1.9/doc/terminology.rst`

 * *Files identical despite different names*

### Comparing `productmd-1.8/doc/images-1.0.rst` & `productmd-1.9/doc/images-1.0.rst`

 * *Files identical despite different names*

### Comparing `productmd-1.8/doc/composeinfo.rst` & `productmd-1.9/doc/composeinfo.rst`

 * *Files identical despite different names*

### Comparing `productmd-1.8/doc/index.rst` & `productmd-1.9/doc/index.rst`

 * *Files identical despite different names*

### Comparing `productmd-1.8/doc/treeinfo.rst` & `productmd-1.9/doc/treeinfo.rst`

 * *Files identical despite different names*

### Comparing `productmd-1.8/doc/rpms-1.1.rst` & `productmd-1.9/doc/rpms-1.1.rst`

 * *Files identical despite different names*

### Comparing `productmd-1.8/doc/treeinfo-1.1.rst` & `productmd-1.9/doc/treeinfo-1.1.rst`

 * *Files identical despite different names*

### Comparing `productmd-1.8/Makefile` & `productmd-1.9/Makefile`

 * *Files identical despite different names*

### Comparing `productmd-1.8/productmd/__init__.py` & `productmd-1.9/productmd/__init__.py`

 * *Files identical despite different names*

### Comparing `productmd-1.8/productmd/treeinfo.py` & `productmd-1.9/productmd/treeinfo.py`

 * *Files identical despite different names*

### Comparing `productmd-1.8/productmd/discinfo.py` & `productmd-1.9/productmd/discinfo.py`

 * *Files identical despite different names*

### Comparing `productmd-1.8/productmd/common.py` & `productmd-1.9/productmd/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,14 +102,15 @@
 
 
 #: Supported release types.
 RELEASE_TYPES = [
     "fast",
     "ga",
     "updates",
+    "updates-testing",
     "eus",
     "aus",
     "els",
 ]
 
 
 def is_valid_release_short(short):
```

### Comparing `productmd-1.8/productmd/compose.py` & `productmd-1.9/productmd/compose.py`

 * *Files identical despite different names*

### Comparing `productmd-1.8/productmd/composeinfo.py` & `productmd-1.9/productmd/composeinfo.py`

 * *Files identical despite different names*

### Comparing `productmd-1.8/productmd/images.py` & `productmd-1.9/productmd/images.py`

 * *Files identical despite different names*

### Comparing `productmd-1.8/productmd/rpms.py` & `productmd-1.9/productmd/rpms.py`

 * *Files identical despite different names*

### Comparing `productmd-1.8/setup.py` & `productmd-1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         if "__init__.py" in files:
             packages.add(root.replace("/", "."))
 packages = sorted(packages)
 
 
 setup(
     name            = "productmd",
-    version         = "1.8",
+    version         = "1.9",
     description     = "Product, compose and installation media metadata library",
     url             = "https://github.com/release-engineering/productmd",
     author          = "Daniel Mach",
     author_email    = "dmach@redhat.com",
     license         = "LGPLv2.1",
 
     packages        = packages,
```

### Comparing `productmd-1.8/tests/test_rpms.py` & `productmd-1.9/tests/test_rpms.py`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/test_compose.py` & `productmd-1.9/tests/test_compose.py`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/test_common.py` & `productmd-1.9/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/test_discinfo.py` & `productmd-1.9/tests/test_discinfo.py`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/test_treeinfo.py` & `productmd-1.9/tests/test_treeinfo.py`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/images/f23.json` & `productmd-1.9/tests/images/f23.json`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/images/src_move_before.json` & `productmd-1.9/tests/images/src_move_before.json`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/images/f20.json` & `productmd-1.9/tests/images/f20.json`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/images/src_move_after.json` & `productmd-1.9/tests/images/src_move_after.json`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/test_images.py` & `productmd-1.9/tests/test_images.py`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/test_header.py` & `productmd-1.9/tests/test_header.py`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/test_composeinfo.py` & `productmd-1.9/tests/test_composeinfo.py`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/treeinfo/fedora-16-Fedora.x86_64` & `productmd-1.9/tests/treeinfo/fedora-16-Fedora.x86_64`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/treeinfo/fedora-16-Fedora.i386` & `productmd-1.9/tests/treeinfo/fedora-16-Fedora.i386`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/treeinfo/fedora-19-Fedora.x86_64` & `productmd-1.9/tests/treeinfo/fedora-19-Fedora.x86_64`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/treeinfo/fedora-21-Server.x86_64` & `productmd-1.9/tests/treeinfo/fedora-21-Server.x86_64`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/treeinfo/fedora-14-Fedora.i386` & `productmd-1.9/tests/treeinfo/fedora-14-Fedora.i386`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/treeinfo/fedora-21-Alpha-Cloud.x86_64` & `productmd-1.9/tests/treeinfo/fedora-21-Alpha-Cloud.x86_64`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/treeinfo/fedora-16-Everything.i386` & `productmd-1.9/tests/treeinfo/fedora-16-Everything.i386`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/treeinfo/fedora-20-Fedora.armhfp` & `productmd-1.9/tests/treeinfo/fedora-20-Fedora.armhfp`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/treeinfo/fedora-11-Fedora.x86_64` & `productmd-1.9/tests/treeinfo/fedora-11-Fedora.x86_64`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/treeinfo/fedora-21-Cloud.x86_64` & `productmd-1.9/tests/treeinfo/fedora-21-Cloud.x86_64`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/treeinfo/fedora-21-Alpha-Cloud.i386` & `productmd-1.9/tests/treeinfo/fedora-21-Alpha-Cloud.i386`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/treeinfo/fedora-21-Alpha-Workstation.armhfp` & `productmd-1.9/tests/treeinfo/fedora-21-Alpha-Workstation.armhfp`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/treeinfo/fedora-13-Fedora.x86_64` & `productmd-1.9/tests/treeinfo/fedora-13-Fedora.x86_64`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/treeinfo/fedora-17-Fedora.i386` & `productmd-1.9/tests/treeinfo/fedora-17-Fedora.i386`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/treeinfo/fedora-10-Fedora.ppc` & `productmd-1.9/tests/treeinfo/fedora-10-Fedora.ppc`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/treeinfo/fedora-21-Alpha-Workstation.x86_64` & `productmd-1.9/tests/treeinfo/fedora-21-Alpha-Workstation.x86_64`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/treeinfo/fedora-21-Cloud.armhfp` & `productmd-1.9/tests/treeinfo/fedora-21-Cloud.armhfp`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/treeinfo/fedora-21-Server.i386` & `productmd-1.9/tests/treeinfo/fedora-21-Server.i386`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/treeinfo/fedora-20-Fedora.x86_64` & `productmd-1.9/tests/treeinfo/fedora-20-Fedora.x86_64`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/treeinfo/fedora-17-Fedora.x86_64` & `productmd-1.9/tests/treeinfo/fedora-17-Fedora.x86_64`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/treeinfo/fedora-11-Fedora.ppc` & `productmd-1.9/tests/treeinfo/fedora-11-Fedora.ppc`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/treeinfo/fedora-16-Everything.x86_64` & `productmd-1.9/tests/treeinfo/fedora-16-Everything.x86_64`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/treeinfo/fedora-18-Fedora.x86_64` & `productmd-1.9/tests/treeinfo/fedora-18-Fedora.x86_64`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/treeinfo/fedora-14-Fedora.x86_64` & `productmd-1.9/tests/treeinfo/fedora-14-Fedora.x86_64`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/treeinfo/fedora-11-Fedora.i386` & `productmd-1.9/tests/treeinfo/fedora-11-Fedora.i386`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/treeinfo/fedora-21-Alpha-Server.i386` & `productmd-1.9/tests/treeinfo/fedora-21-Alpha-Server.i386`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/treeinfo/fedora-15-Fedora.x86_64` & `productmd-1.9/tests/treeinfo/fedora-15-Fedora.x86_64`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/treeinfo/fedora-21-Server.armhfp` & `productmd-1.9/tests/treeinfo/fedora-21-Server.armhfp`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/treeinfo/fedora-10-Fedora.x86_64` & `productmd-1.9/tests/treeinfo/fedora-10-Fedora.x86_64`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/treeinfo/fedora-21-Alpha-Cloud.armhfp` & `productmd-1.9/tests/treeinfo/fedora-21-Alpha-Cloud.armhfp`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/treeinfo/fedora-12-Fedora.ppc` & `productmd-1.9/tests/treeinfo/fedora-12-Fedora.ppc`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/treeinfo/fedora-18-Everything.x86_64` & `productmd-1.9/tests/treeinfo/fedora-18-Everything.x86_64`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/treeinfo/fedora-12-Fedora.x86_64` & `productmd-1.9/tests/treeinfo/fedora-12-Fedora.x86_64`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/treeinfo/fedora-21-Alpha-Server.armhfp` & `productmd-1.9/tests/treeinfo/fedora-21-Alpha-Server.armhfp`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/treeinfo/fedora-12-Fedora.i386` & `productmd-1.9/tests/treeinfo/fedora-12-Fedora.i386`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/treeinfo/fedora-13-Fedora.i386` & `productmd-1.9/tests/treeinfo/fedora-13-Fedora.i386`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/treeinfo/fedora-15-Fedora.i386` & `productmd-1.9/tests/treeinfo/fedora-15-Fedora.i386`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/treeinfo/fedora-18-Everything.i386` & `productmd-1.9/tests/treeinfo/fedora-18-Everything.i386`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/treeinfo/fedora-10-Fedora.i386` & `productmd-1.9/tests/treeinfo/fedora-10-Fedora.i386`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/treeinfo/fedora-19-Fedora.i386` & `productmd-1.9/tests/treeinfo/fedora-19-Fedora.i386`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/treeinfo/fedora-21-Alpha-Workstation.i386` & `productmd-1.9/tests/treeinfo/fedora-21-Alpha-Workstation.i386`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/treeinfo/fedora-21-Alpha-Server.x86_64` & `productmd-1.9/tests/treeinfo/fedora-21-Alpha-Server.x86_64`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/treeinfo/fedora-21-Cloud.i386` & `productmd-1.9/tests/treeinfo/fedora-21-Cloud.i386`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/treeinfo/fedora-18-Fedora.i386` & `productmd-1.9/tests/treeinfo/fedora-18-Fedora.i386`

 * *Files identical despite different names*

### Comparing `productmd-1.8/tests/treeinfo/fedora-20-Fedora.i386` & `productmd-1.9/tests/treeinfo/fedora-20-Fedora.i386`

 * *Files identical despite different names*

### Comparing `productmd-1.8/LICENSE` & `productmd-1.9/LICENSE`

 * *Files identical despite different names*

