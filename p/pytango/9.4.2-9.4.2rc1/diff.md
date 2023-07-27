# Comparing `tmp/pytango-9.4.2.tar.gz` & `tmp/pytango-9.4.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytango-9.4.2.tar", last modified: Thu Jul 27 14:21:27 2023, max compression
+gzip compressed data, was "pytango-9.4.2rc1.tar", last modified: Thu Jul 13 09:38:37 2023, max compression
```

## Comparing `pytango-9.4.2.tar` & `pytango-9.4.2rc1.tar`

### file list

```diff
@@ -1,408 +1,412 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:21:27.754733 pytango-9.4.2/
--rw-rw-rw-   0 root         (0) root         (0)     6685 2023-07-21 16:54:44.000000 pytango-9.4.2/CMakeLists.txt
--rw-rw-rw-   0 root         (0) root         (0)     7883 2023-06-30 12:46:38.000000 pytango-9.4.2/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)      267 2023-07-21 16:54:44.000000 pytango-9.4.2/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     8584 2023-07-21 16:54:44.000000 pytango-9.4.2/Makefile
--rw-r--r--   0 root         (0) root         (0)     6383 2023-07-27 14:21:27.754733 pytango-9.4.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1560 2023-02-24 12:24:40.000000 pytango-9.4.2/PyTango.py
--rw-rw-rw-   0 root         (0) root         (0)     5027 2023-07-21 16:54:44.000000 pytango-9.4.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:21:27.681733 pytango-9.4.2/cmake/
--rw-rw-rw-   0 root         (0) root         (0)      814 2023-02-24 12:24:40.000000 pytango-9.4.2/cmake/project_version.cc.in
--rw-rw-rw-   0 root         (0) root         (0)     7407 2023-02-24 12:24:40.000000 pytango-9.4.2/cmake/project_version.cmake
--rw-rw-rw-   0 root         (0) root         (0)     1672 2023-02-24 12:24:40.000000 pytango-9.4.2/cmake/project_version.h.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:21:27.686733 pytango-9.4.2/doc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:21:27.687733 pytango-9.4.2/doc/.devcontainer/
--rw-rw-rw-   0 root         (0) root         (0)      314 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/.devcontainer/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)     1484 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/.devcontainer/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:21:27.699733 pytango-9.4.2/doc/_static/
--rw-rw-rw-   0 root         (0) root         (0)     5669 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/_static/arrow03.png
--rw-rw-rw-   0 root         (0) root         (0)   237697 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/_static/banner1.png
--rw-rw-rw-   0 root         (0) root         (0)    73015 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/_static/banner2.png
--rw-rw-rw-   0 root         (0) root         (0)    83303 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/_static/banner3.png
--rw-rw-rw-   0 root         (0) root         (0)     7419 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/_static/boost_python_install.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:21:27.699733 pytango-9.4.2/doc/_static/css/
--rw-rw-rw-   0 root         (0) root         (0)   132306 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/_static/css/tango_cs_theme.css
--rw-rw-rw-   0 root         (0) root         (0)    13726 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/_static/database.png
--rw-rw-rw-   0 root         (0) root         (0)    65909 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/_static/device.png
--rw-rw-rw-   0 root         (0) root         (0)     1104 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/_static/gallery.js
--rw-rw-rw-   0 root         (0) root         (0)   603593 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/_static/green_python.png
--rw-rw-rw-   0 root         (0) root         (0)  1684994 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/_static/green_python_original.png
--rw-rw-rw-   0 root         (0) root         (0)     2765 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/_static/ipython_db.html
--rw-rw-rw-   0 root         (0) root         (0)     3829 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/_static/ipython_motor.html
--rw-rw-rw-   0 root         (0) root         (0)     3909 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/_static/ipython_serial.html
--rw-rw-rw-   0 root         (0) root         (0)    20483 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/_static/ipython_tango.html
--rw-rw-rw-   0 root         (0) root         (0)    30674 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/_static/itango00.png
--rw-rw-rw-   0 root         (0) root         (0)    14791 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/_static/jive_powersupply.png
--rw-rw-rw-   0 root         (0) root         (0)      769 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/_static/jssor.css
--rw-rw-rw-   0 root         (0) root         (0)    92207 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/_static/jssor.js
--rw-rw-rw-   0 root         (0) root         (0)   170401 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/_static/jssor.slider.js
--rw-rw-rw-   0 root         (0) root         (0)   172668 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/_static/logo-medium.png
--rwxrwxrwx   0 root         (0) root         (0)     4030 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/_static/logo.ico
--rw-rw-rw-   0 root         (0) root         (0)    99573 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/_static/logo.png
--rw-rw-rw-   0 root         (0) root         (0)   221457 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/_static/mocking-tango-db-access-crossed-out.png
--rw-rw-rw-   0 root         (0) root         (0)   145562 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/_static/mocking-tango-db-access.png
--rw-rw-rw-   0 root         (0) root         (0)    63184 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/_static/mocking-tango-test-case-not-mocked.png
--rw-rw-rw-   0 root         (0) root         (0)    54671 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/_static/mocking-tango-test-case-real-vs-mocked.png
--rw-rw-rw-   0 root         (0) root         (0)   179107 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/_static/mocking-tango-test-doubles.png
--rw-rw-rw-   0 root         (0) root         (0)    13299 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/_static/motor.png
--rw-rw-rw-   0 root         (0) root         (0)     2455 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/_static/power_supply.py
--rw-rw-rw-   0 root         (0) root         (0)      891 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/_static/project-config.jam
--rw-rw-rw-   0 root         (0) root         (0)     6201 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/_static/pytango.css
--rw-rw-rw-   0 root         (0) root         (0)     6323 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/_static/serial.png
--rw-rw-rw-   0 root         (0) root         (0)      720 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/_static/slideshow.js
--rw-rw-rw-   0 root         (0) root         (0)    15763 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/_static/starter.png
--rw-rw-rw-   0 root         (0) root         (0)   171117 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/_static/testing-approaches-device-test-context-x2.png
--rw-rw-rw-   0 root         (0) root         (0)   211964 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/_static/testing-approaches-device-test-context.png
--rw-rw-rw-   0 root         (0) root         (0)   206869 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/_static/testing-approaches-hybrid.png
--rw-rw-rw-   0 root         (0) root         (0)   336790 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/_static/testing-approaches-multi-device-test-context.png
--rw-rw-rw-   0 root         (0) root         (0)   108016 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/_static/testing-approaches-real-facility.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:21:27.700733 pytango-9.4.2/doc/_templates/
--rw-rw-rw-   0 root         (0) root         (0)      695 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/_templates/breadcrumbs.html
--rw-rw-rw-   0 root         (0) root         (0)    14238 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/_templates/index.html
--rw-rw-rw-   0 root         (0) root         (0)      642 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/_templates/indexsidebar.html
--rw-rw-rw-   0 root         (0) root         (0)      246 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/api.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:21:27.701733 pytango-9.4.2/doc/client_api/
--rw-rw-rw-   0 root         (0) root         (0)      111 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/client_api/attribute_proxy.rst
--rw-rw-rw-   0 root         (0) root         (0)      187 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/client_api/device_proxy.rst
--rw-rw-rw-   0 root         (0) root         (0)      474 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/client_api/green.rst
--rw-rw-rw-   0 root         (0) root         (0)     1157 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/client_api/group.rst
--rw-rw-rw-   0 root         (0) root         (0)      139 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/client_api/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     2410 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/client_api/miscellaneous.rst
--rw-rw-rw-   0 root         (0) root         (0)     1056 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/client_api/other.rst
--rw-rw-rw-   0 root         (0) root         (0)    18665 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      423 2023-06-30 12:46:38.000000 pytango-9.4.2/doc/contents.rst
--rw-rw-rw-   0 root         (0) root         (0)    42078 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/data_types.rst
--rw-rw-rw-   0 root         (0) root         (0)      493 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/database.rst
--rw-rw-rw-   0 root         (0) root         (0)      171 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/encoded.rst
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-07-08 16:38:26.000000 pytango-9.4.2/doc/environment.yml
--rw-rw-rw-   0 root         (0) root         (0)    12704 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/exception.rst
--rw-rw-rw-   0 root         (0) root         (0)     1508 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/faq.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:21:27.702733 pytango-9.4.2/doc/green_modes/
--rw-rw-rw-   0 root         (0) root         (0)      525 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/green_modes/client_asyncio_mode.rst
--rw-rw-rw-   0 root         (0) root         (0)     3542 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/green_modes/client_futures_mode.rst
--rw-rw-rw-   0 root         (0) root         (0)     4036 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/green_modes/client_gevent_mode.rst
--rw-rw-rw-   0 root         (0) root         (0)     1220 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/green_modes/green.rst
--rw-rw-rw-   0 root         (0) root         (0)     1204 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/green_modes/green_modes_client.rst
--rw-rw-rw-   0 root         (0) root         (0)     2473 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/green_modes/green_modes_server.rst
--rw-rw-rw-   0 root         (0) root         (0)     9922 2023-07-21 16:54:44.000000 pytango-9.4.2/doc/how-to-contribute.rst
--rw-rw-rw-   0 root         (0) root         (0)    62310 2023-07-11 14:59:09.000000 pytango-9.4.2/doc/howto.rst
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/indexes.rst
--rw-rw-rw-   0 root         (0) root         (0)      524 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/itango.rst
--rw-rw-rw-   0 root         (0) root         (0)   206038 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/logo-medium.bmp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:21:27.702733 pytango-9.4.2/doc/man/
--rw-rw-rw-   0 root         (0) root         (0)      451 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/man/itango.1
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:21:27.702733 pytango-9.4.2/doc/migration/
--rw-rw-rw-   0 root         (0) root         (0)      212 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/migration/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:21:27.704733 pytango-9.4.2/doc/migration/to-9.4/
--rw-rw-rw-   0 root         (0) root         (0)     1566 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/migration/to-9.4/attr-decorators.rst
--rw-rw-rw-   0 root         (0) root         (0)     1156 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/migration/to-9.4/deps-install.rst
--rw-rw-rw-   0 root         (0) root         (0)    16392 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/migration/to-9.4/empty-attrs.rst
--rw-rw-rw-   0 root         (0) root         (0)     2033 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/migration/to-9.4/extract-as.rst
--rw-rw-rw-   0 root         (0) root         (0)     2075 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/migration/to-9.4/hl-dev-enum.rst
--rw-rw-rw-   0 root         (0) root         (0)      756 2023-03-03 08:48:14.000000 pytango-9.4.2/doc/migration/to-9.4/hl-dynamic.rst
--rw-rw-rw-   0 root         (0) root         (0)      377 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/migration/to-9.4/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1344 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/migration/to-9.4/logging-percent-sym.rst
--rw-rw-rw-   0 root         (0) root         (0)     3887 2023-03-03 08:48:14.000000 pytango-9.4.2/doc/migration/to-9.4/non-bound-user-funcs.rst
--rw-rw-rw-   0 root         (0) root         (0)     1997 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/migration/to-9.4/optional-proxy-attrs.rst
--rw-rw-rw-   0 root         (0) root         (0)     5186 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/mock_tango_extension.py
--rw-rw-rw-   0 root         (0) root         (0)     8020 2023-07-27 12:24:43.000000 pytango-9.4.2/doc/news.rst
--rw-rw-rw-   0 root         (0) root         (0)     9178 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/quicktour.rst
--rw-rw-rw-   0 root         (0) root         (0)   171205 2023-07-27 12:37:05.000000 pytango-9.4.2/doc/revision.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:21:27.706733 pytango-9.4.2/doc/server_api/
--rw-rw-rw-   0 root         (0) root         (0)      434 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/server_api/attribute.rst
--rw-rw-rw-   0 root         (0) root         (0)      141 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/server_api/device.rst
--rw-rw-rw-   0 root         (0) root         (0)       98 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/server_api/device_class.rst
--rw-rw-rw-   0 root         (0) root         (0)      158 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/server_api/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      419 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/server_api/logging.rst
--rw-rw-rw-   0 root         (0) root         (0)    10620 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/server_api/server.rst
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/server_api/util.rst
--rw-rw-rw-   0 root         (0) root         (0)     6458 2023-07-21 16:54:44.000000 pytango-9.4.2/doc/start.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:21:27.707733 pytango-9.4.2/doc/tep/
--rw-rw-rw-   0 root         (0) root         (0)    56811 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/tep/DataBase.xmi
--rw-rw-rw-   0 root         (0) root         (0)   100867 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/tep/database.py
--rw-rw-rw-   0 root         (0) root         (0)    19326 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/tep/tep-0001.rst
--rw-rw-rw-   0 root         (0) root         (0)    17205 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/tep/tep-0002.rst
--rw-rw-rw-   0 root         (0) root         (0)      222 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/tep.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:21:27.707733 pytango-9.4.2/doc/testing/
--rw-rw-rw-   0 root         (0) root         (0)     3725 2023-07-21 16:54:44.000000 pytango-9.4.2/doc/testing/coverage.rst
--rw-rw-rw-   0 root         (0) root         (0)     8724 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/testing/mocks.rst
--rw-rw-rw-   0 root         (0) root         (0)      643 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/testing/test_context.rst
--rw-rw-rw-   0 root         (0) root         (0)    15469 2023-07-21 16:54:44.000000 pytango-9.4.2/doc/testing/testing_approaches.rst
--rw-rw-rw-   0 root         (0) root         (0)      276 2023-07-21 16:54:44.000000 pytango-9.4.2/doc/testing.rst
--rw-rw-rw-   0 root         (0) root         (0)     1088 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/utilities.rst
--rw-rw-rw-   0 root         (0) root         (0)     2400 2023-06-30 12:46:38.000000 pytango-9.4.2/doc/version-policy.rst
--rw-rw-rw-   0 root         (0) root         (0)     6737 2023-02-24 12:24:40.000000 pytango-9.4.2/doc/windows_notes.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:21:27.675733 pytango-9.4.2/examples/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:21:27.708733 pytango-9.4.2/examples/Clock/
--rw-rw-rw-   0 root         (0) root         (0)      315 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/Clock/Clock.py
--rw-rw-rw-   0 root         (0) root         (0)     1867 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/Clock/ClockDS.py
--rw-rw-rw-   0 root         (0) root         (0)     1490 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/Clock/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:21:27.708733 pytango-9.4.2/examples/TuringMachine/
--rw-rw-rw-   0 root         (0) root         (0)     2062 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/TuringMachine/TuringMachine.py
--rw-rw-rw-   0 root         (0) root         (0)      447 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/TuringMachine/turing_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:21:27.709733 pytango-9.4.2/examples/asyncio_green_mode/
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/asyncio_green_mode/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      969 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/asyncio_green_mode/asyncio_device_example.py
--rw-rw-rw-   0 root         (0) root         (0)      281 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/asyncio_green_mode/asyncio_simple_example.py
--rw-rw-rw-   0 root         (0) root         (0)     1886 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/asyncio_green_mode/tcp_server_example.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:21:27.709733 pytango-9.4.2/examples/dynamic/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:21:27.710733 pytango-9.4.2/examples/dynamic/common/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-27 14:21:09.000000 pytango-9.4.2/examples/dynamic/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      285 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/dynamic/common/roi.py
--rw-rw-rw-   0 root         (0) root         (0)      638 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/dynamic/dynamic_client.py
--rw-rw-rw-   0 root         (0) root         (0)      958 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/dynamic/dynamic_server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:21:27.710733 pytango-9.4.2/examples/fwdAttr/
--rw-rw-rw-   0 root         (0) root         (0)      883 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/fwdAttr/FwdServer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:21:27.712733 pytango-9.4.2/examples/interfacechangeEvents/
--rw-rw-rw-   0 root         (0) root         (0)     1954 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/interfacechangeEvents/ClassFactory.cpp
--rw-rw-rw-   0 root         (0) root         (0)     1841 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/interfacechangeEvents/IfchangeClient.py
--rw-rw-rw-   0 root         (0) root         (0)    11392 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/interfacechangeEvents/IfchangeServer.cpp
--rw-rw-rw-   0 root         (0) root         (0)     5744 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/interfacechangeEvents/IfchangeServer.h
--rw-rw-rw-   0 root         (0) root         (0)     1926 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/interfacechangeEvents/IfchangeServer.py
--rw-rw-rw-   0 root         (0) root         (0)     4643 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/interfacechangeEvents/IfchangeServer.xmi
--rw-rw-rw-   0 root         (0) root         (0)    21544 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/interfacechangeEvents/IfchangeServerClass.cpp
--rw-rw-rw-   0 root         (0) root         (0)     7254 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/interfacechangeEvents/IfchangeServerClass.h
--rw-rw-rw-   0 root         (0) root         (0)     6341 2023-07-27 08:42:45.000000 pytango-9.4.2/examples/interfacechangeEvents/IfchangeServerDynAttrUtils.cpp
--rw-rw-rw-   0 root         (0) root         (0)     5037 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/interfacechangeEvents/IfchangeServerStateMachine.cpp
--rw-rw-rw-   0 root         (0) root         (0)     5095 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/interfacechangeEvents/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     5095 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/interfacechangeEvents/Makefile.bck
--rw-rw-rw-   0 root         (0) root         (0)     2731 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/interfacechangeEvents/main.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:21:27.712733 pytango-9.4.2/examples/mandatory/
--rw-rw-rw-   0 root         (0) root         (0)      576 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/mandatory/MandatoryPropertyServer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:21:27.713733 pytango-9.4.2/examples/many/
--rw-rw-rw-   0 root         (0) root         (0)      388 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/many/many_client.py
--rw-rw-rw-   0 root         (0) root         (0)      685 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/many/many_server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:21:27.713733 pytango-9.4.2/examples/multi/
--rw-rw-rw-   0 root         (0) root         (0)      700 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/multi/multi_client.py
--rw-rw-rw-   0 root         (0) root         (0)      955 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/multi/multi_server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:21:27.714733 pytango-9.4.2/examples/multidevicetestcontext/
--rw-rw-rw-   0 root         (0) root         (0)      960 2023-07-06 14:21:46.000000 pytango-9.4.2/examples/multidevicetestcontext/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     2763 2023-07-06 14:21:46.000000 pytango-9.4.2/examples/multidevicetestcontext/test_integration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:21:27.715733 pytango-9.4.2/examples/pipeEvents/
--rw-rw-rw-   0 root         (0) root         (0)     1926 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/pipeEvents/ClassFactory.cpp
--rw-rw-rw-   0 root         (0) root         (0)     5047 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/pipeEvents/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     1579 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/pipeEvents/PipeEventClient.py
--rw-rw-rw-   0 root         (0) root         (0)    15129 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/pipeEvents/PipeServer.cpp
--rw-rw-rw-   0 root         (0) root         (0)     4833 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/pipeEvents/PipeServer.h
--rw-rw-rw-   0 root         (0) root         (0)     2977 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/pipeEvents/PipeServer.py
--rw-rw-rw-   0 root         (0) root         (0)     2512 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/pipeEvents/PipeServer.xmi
--rw-rw-rw-   0 root         (0) root         (0)    19277 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/pipeEvents/PipeServerClass.cpp
--rw-rw-rw-   0 root         (0) root         (0)     5100 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/pipeEvents/PipeServerClass.h
--rw-rw-rw-   0 root         (0) root         (0)     3687 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/pipeEvents/PipeServerStateMachine.cpp
--rw-rw-rw-   0 root         (0) root         (0)     2719 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/pipeEvents/main.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:21:27.717733 pytango-9.4.2/examples/pipes/
--rw-rw-rw-   0 root         (0) root         (0)     1926 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/pipes/ClassFactory.cpp
--rw-rw-rw-   0 root         (0) root         (0)     5047 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/pipes/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      893 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/pipes/PipeClient.py
--rw-rw-rw-   0 root         (0) root         (0)    11859 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/pipes/PipeServer.cpp
--rw-rw-rw-   0 root         (0) root         (0)     4416 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/pipes/PipeServer.h
--rw-rw-rw-   0 root         (0) root         (0)     1031 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/pipes/PipeServer.py
--rw-rw-rw-   0 root         (0) root         (0)     2089 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/pipes/PipeServer.xmi
--rw-rw-rw-   0 root         (0) root         (0)    18280 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/pipes/PipeServerClass.cpp
--rw-rw-rw-   0 root         (0) root         (0)     4186 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/pipes/PipeServerClass.h
--rw-rw-rw-   0 root         (0) root         (0)     3082 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/pipes/PipeServerStateMachine.cpp
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-27 14:21:09.000000 pytango-9.4.2/examples/pipes/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2719 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/pipes/main.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:21:27.718733 pytango-9.4.2/examples/simple/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:21:27.718733 pytango-9.4.2/examples/simple/common/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-27 14:21:09.000000 pytango-9.4.2/examples/simple/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      285 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/simple/common/roi.py
--rw-rw-rw-   0 root         (0) root         (0)      638 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/simple/simple_client.py
--rw-rw-rw-   0 root         (0) root         (0)      963 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/simple/simple_server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:21:27.718733 pytango-9.4.2/examples/training/
--rw-rw-rw-   0 root         (0) root         (0)     5106 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/training/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:21:27.720733 pytango-9.4.2/examples/training/client/
--rwxrwxrwx   0 root         (0) root         (0)     1784 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/training/client/command01.py
--rwxrwxrwx   0 root         (0) root         (0)     1815 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/training/client/command02.py
--rwxrwxrwx   0 root         (0) root         (0)     1185 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/training/client/reading01.py
--rwxrwxrwx   0 root         (0) root         (0)     1636 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/training/client/reading02.py
--rwxrwxrwx   0 root         (0) root         (0)     5644 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/training/client/reading03.py
--rwxrwxrwx   0 root         (0) root         (0)     1251 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/training/client/writing01.py
--rwxrwxrwx   0 root         (0) root         (0)     1260 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/training/client/writing02.py
--rw-rw-rw-   0 root         (0) root         (0)     2444 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/training/docker-compose.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:21:27.722733 pytango-9.4.2/examples/training/server/
--rwxrwxrwx   0 root         (0) root         (0)      412 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/training/server/high-level-api.py
--rwxrwxrwx   0 root         (0) root         (0)     1331 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/training/server/libps.py
--rwxrwxrwx   0 root         (0) root         (0)     1340 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/training/server/low-level-api.py
--rwxrwxrwx   0 root         (0) root         (0)     3831 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/training/server/ps-simulator.py
--rwxrwxrwx   0 root         (0) root         (0)      394 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/training/server/ps0a.py
--rwxrwxrwx   0 root         (0) root         (0)     1058 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/training/server/ps0b-push-event.py
--rwxrwxrwx   0 root         (0) root         (0)      623 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/training/server/ps0b.py
--rwxrwxrwx   0 root         (0) root         (0)     1216 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/training/server/ps0c.py
--rwxrwxrwx   0 root         (0) root         (0)     1217 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/training/server/ps1-gevent.py
--rwxrwxrwx   0 root         (0) root         (0)     1154 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/training/server/ps1-use-lib-logging.py
--rwxrwxrwx   0 root         (0) root         (0)      943 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/training/server/ps1-use-lib.py
--rwxrwxrwx   0 root         (0) root         (0)     1119 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/training/server/ps1.py
--rwxrwxrwx   0 root         (0) root         (0)     1770 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/training/server/ps2-gevent-check.py
--rwxrwxrwx   0 root         (0) root         (0)     1462 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/training/server/ps2-gevent.py
--rw-rw-rw-   0 root         (0) root         (0)      351 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/training/server/test_ps0a.py
--rw-rw-rw-   0 root         (0) root         (0)      929 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/training/server/test_ps0b.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:21:27.723733 pytango-9.4.2/examples/training/webinars/
--rw-rw-rw-   0 root         (0) root         (0)      648 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/training/webinars/crash_example.py
--rw-rw-rw-   0 root         (0) root         (0)     3557 2023-02-24 12:24:40.000000 pytango-9.4.2/examples/training/webinars/test_webinar.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:21:27.735733 pytango-9.4.2/ext/
--rw-rw-rw-   0 root         (0) root         (0)     2498 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/api_util.cpp
--rw-rw-rw-   0 root         (0) root         (0)     1102 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/archive_event_info.cpp
--rw-rw-rw-   0 root         (0) root         (0)     2618 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/attr_conf_event_data.cpp
--rw-rw-rw-   0 root         (0) root         (0)     1299 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/attribute_alarm_info.cpp
--rw-rw-rw-   0 root         (0) root         (0)      872 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/attribute_dimension.cpp
--rw-rw-rw-   0 root         (0) root         (0)      989 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/attribute_event_info.cpp
--rw-rw-rw-   0 root         (0) root         (0)      921 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/attribute_info.cpp
--rw-rw-rw-   0 root         (0) root         (0)     1276 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/attribute_info_ex.cpp
--rw-rw-rw-   0 root         (0) root         (0)     4095 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/attribute_proxy.cpp
--rw-rw-rw-   0 root         (0) root         (0)    16584 2023-06-30 12:46:38.000000 pytango-9.4.2/ext/base_types.cpp
--rw-rw-rw-   0 root         (0) root         (0)     3388 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/base_types_numpy.hpp
--rw-rw-rw-   0 root         (0) root         (0)    15060 2023-03-03 08:48:14.000000 pytango-9.4.2/ext/callback.cpp
--rw-rw-rw-   0 root         (0) root         (0)     4682 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/callback.h
--rw-rw-rw-   0 root         (0) root         (0)      981 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/change_event_info.cpp
--rw-rw-rw-   0 root         (0) root         (0)      824 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/command_info.cpp
--rw-rw-rw-   0 root         (0) root         (0)     5786 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/connection.cpp
--rw-rw-rw-   0 root         (0) root         (0)    18026 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/constants.cpp
--rw-rw-rw-   0 root         (0) root         (0)     2842 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/data_ready_event_data.cpp
--rw-rw-rw-   0 root         (0) root         (0)    19287 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/database.cpp
--rw-rw-rw-   0 root         (0) root         (0)     4296 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/db.cpp
--rw-rw-rw-   0 root         (0) root         (0)     1228 2023-03-03 08:48:14.000000 pytango-9.4.2/ext/defs.h
--rw-rw-rw-   0 root         (0) root         (0)     1321 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/dev_command_info.cpp
--rw-rw-rw-   0 root         (0) root         (0)     2172 2023-06-30 12:46:38.000000 pytango-9.4.2/ext/dev_error.cpp
--rw-rw-rw-   0 root         (0) root         (0)    33447 2023-06-30 12:46:38.000000 pytango-9.4.2/ext/device_attribute.cpp
--rw-rw-rw-   0 root         (0) root         (0)     7614 2023-06-30 12:46:38.000000 pytango-9.4.2/ext/device_attribute.h
--rw-rw-rw-   0 root         (0) root         (0)     2667 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/device_attribute_config.cpp
--rw-rw-rw-   0 root         (0) root         (0)     1013 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/device_attribute_history.cpp
--rw-rw-rw-   0 root         (0) root         (0)    10170 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/device_attribute_numpy.hpp
--rw-rw-rw-   0 root         (0) root         (0)     8332 2023-06-30 12:46:38.000000 pytango-9.4.2/ext/device_data.cpp
--rw-rw-rw-   0 root         (0) root         (0)     1185 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/device_data_history.cpp
--rw-rw-rw-   0 root         (0) root         (0)     1120 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/device_info.cpp
--rw-rw-rw-   0 root         (0) root         (0)    14245 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/device_pipe.cpp
--rw-rw-rw-   0 root         (0) root         (0)     1743 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/device_pipe.h
--rw-rw-rw-   0 root         (0) root         (0)    42737 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/device_proxy.cpp
--rw-rw-rw-   0 root         (0) root         (0)     2898 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/devintr_change_event_data.cpp
--rw-rw-rw-   0 root         (0) root         (0)    12739 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/enums.cpp
--rw-rw-rw-   0 root         (0) root         (0)     2951 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/event_data.cpp
--rw-rw-rw-   0 root         (0) root         (0)    18550 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/exception.cpp
--rw-rw-rw-   0 root         (0) root         (0)     3594 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/exception.h
--rw-rw-rw-   0 root         (0) root         (0)    18306 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/fast_from_py.h
--rw-rw-rw-   0 root         (0) root         (0)     9248 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/fast_from_py_numpy.hpp
--rw-rw-rw-   0 root         (0) root         (0)    16044 2023-06-30 12:46:38.000000 pytango-9.4.2/ext/from_py.cpp
--rw-rw-rw-   0 root         (0) root         (0)    26882 2023-06-30 12:46:38.000000 pytango-9.4.2/ext/from_py.h
--rw-rw-rw-   0 root         (0) root         (0)    13470 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/group.cpp
--rw-rw-rw-   0 root         (0) root         (0)     2717 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/group_reply.cpp
--rw-rw-rw-   0 root         (0) root         (0)     1971 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/group_reply_list.cpp
--rw-rw-rw-   0 root         (0) root         (0)     1204 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/locker_info.cpp
--rw-rw-rw-   0 root         (0) root         (0)      725 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/locking_thread.cpp
--rw-rw-rw-   0 root         (0) root         (0)      909 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/periodic_event_info.cpp
--rw-rw-rw-   0 root         (0) root         (0)     2503 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/pipe_event_data.cpp
--rw-rw-rw-   0 root         (0) root         (0)     1151 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/pipe_info.cpp
--rw-rw-rw-   0 root         (0) root         (0)     1047 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/poll_device.cpp
--rw-rw-rw-   0 root         (0) root         (0)      577 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/precompiled_header.cpp
--rw-rw-rw-   0 root         (0) root         (0)     1307 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/precompiled_header.hpp
--rw-rw-rw-   0 root         (0) root         (0)     3343 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/pytango.cpp
--rw-rw-rw-   0 root         (0) root         (0)      652 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/pytgutils.cpp
--rw-rw-rw-   0 root         (0) root         (0)     2021 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/pytgutils.h
--rw-rw-rw-   0 root         (0) root         (0)     8373 2023-06-30 12:46:38.000000 pytango-9.4.2/ext/pyutils.cpp
--rw-rw-rw-   0 root         (0) root         (0)     7427 2023-06-30 12:46:38.000000 pytango-9.4.2/ext/pyutils.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:21:27.740733 pytango-9.4.2/ext/server/
--rw-rw-rw-   0 root         (0) root         (0)    10787 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/server/attr.cpp
--rw-rw-rw-   0 root         (0) root         (0)    10786 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/server/attr.h
--rw-rw-rw-   0 root         (0) root         (0)    34005 2023-06-30 12:46:38.000000 pytango-9.4.2/ext/server/attribute.cpp
--rw-rw-rw-   0 root         (0) root         (0)     2860 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/server/attribute.h
--rw-rw-rw-   0 root         (0) root         (0)     3350 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/server/auto_monitor.cpp
--rw-rw-rw-   0 root         (0) root         (0)    10091 2023-06-30 12:46:38.000000 pytango-9.4.2/ext/server/command.cpp
--rw-rw-rw-   0 root         (0) root         (0)     1665 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/server/command.h
--rw-rw-rw-   0 root         (0) root         (0)    15118 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/server/device_class.cpp
--rw-rw-rw-   0 root         (0) root         (0)     6475 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/server/device_class.h
--rw-rw-rw-   0 root         (0) root         (0)    67588 2023-07-27 08:42:45.000000 pytango-9.4.2/ext/server/device_impl.cpp
--rw-rw-rw-   0 root         (0) root         (0)    13502 2023-07-21 16:54:44.000000 pytango-9.4.2/ext/server/device_impl.h
--rw-rw-rw-   0 root         (0) root         (0)     7705 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/server/dserver.cpp
--rw-rw-rw-   0 root         (0) root         (0)    46343 2023-07-21 16:54:44.000000 pytango-9.4.2/ext/server/encoded_attribute.cpp
--rw-rw-rw-   0 root         (0) root         (0)     1084 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/server/fwdAttr.cpp
--rw-rw-rw-   0 root         (0) root         (0)     6352 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/server/log4tango.cpp
--rw-rw-rw-   0 root         (0) root         (0)     2367 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/server/multi_attribute.cpp
--rw-rw-rw-   0 root         (0) root         (0)     1190 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/server/multi_class_attribute.cpp
--rw-rw-rw-   0 root         (0) root         (0)    19095 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/server/pipe.cpp
--rw-rw-rw-   0 root         (0) root         (0)     2568 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/server/pipe.h
--rw-rw-rw-   0 root         (0) root         (0)     1904 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/server/subdev.cpp
--rw-rw-rw-   0 root         (0) root         (0)    11368 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/server/tango_util.cpp
--rw-rw-rw-   0 root         (0) root         (0)     4608 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/server/user_default_attr_prop.cpp
--rw-rw-rw-   0 root         (0) root         (0)      911 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/server/user_default_pipe_prop.cpp
--rw-rw-rw-   0 root         (0) root         (0)    23854 2023-07-11 14:59:09.000000 pytango-9.4.2/ext/server/wattribute.cpp
--rw-rw-rw-   0 root         (0) root         (0)     2575 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/server/wattribute_numpy.hpp
--rw-rw-rw-   0 root         (0) root         (0)     3003 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/tango_numpy.h
--rw-rw-rw-   0 root         (0) root         (0)    24364 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/tgutils.h
--rw-rw-rw-   0 root         (0) root         (0)      885 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/time_val.cpp
--rw-rw-rw-   0 root         (0) root         (0)    12585 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/to_py.cpp
--rw-rw-rw-   0 root         (0) root         (0)    12370 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/to_py.h
--rw-rw-rw-   0 root         (0) root         (0)     5383 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/to_py_numpy.hpp
--rw-rw-rw-   0 root         (0) root         (0)      723 2023-02-24 12:24:40.000000 pytango-9.4.2/ext/version.cpp
--rw-rw-rw-   0 root         (0) root         (0)      554 2023-07-21 16:54:44.000000 pytango-9.4.2/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:21:27.741733 pytango-9.4.2/pytango.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6383 2023-07-27 14:21:27.000000 pytango-9.4.2/pytango.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    13811 2023-07-27 14:21:27.000000 pytango-9.4.2/pytango.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 14:21:27.000000 pytango-9.4.2/pytango.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       95 2023-07-27 14:21:27.000000 pytango-9.4.2/pytango.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-27 14:21:27.000000 pytango-9.4.2/pytango.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      241 2023-07-27 14:21:27.769733 pytango-9.4.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)    15707 2023-07-21 16:54:44.000000 pytango-9.4.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:21:27.750733 pytango-9.4.2/tango/
--rw-rw-rw-   0 root         (0) root         (0)    10466 2023-02-24 12:24:40.000000 pytango-9.4.2/tango/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5184 2023-02-24 12:24:40.000000 pytango-9.4.2/tango/api_util.py
--rw-rw-rw-   0 root         (0) root         (0)     4464 2023-02-24 12:24:40.000000 pytango-9.4.2/tango/asyncio.py
--rw-rw-rw-   0 root         (0) root         (0)     4016 2023-06-30 12:46:38.000000 pytango-9.4.2/tango/asyncio_executor.py
--rw-rw-rw-   0 root         (0) root         (0)    15383 2023-04-28 08:04:25.000000 pytango-9.4.2/tango/attr_data.py
--rw-rw-rw-   0 root         (0) root         (0)    18234 2023-07-06 14:21:46.000000 pytango-9.4.2/tango/attribute_proxy.py
--rw-rw-rw-   0 root         (0) root         (0)     2092 2023-02-24 12:24:40.000000 pytango-9.4.2/tango/auto_monitor.py
--rw-rw-rw-   0 root         (0) root         (0)    29926 2023-02-24 12:24:40.000000 pytango-9.4.2/tango/base_types.py
--rw-rw-rw-   0 root         (0) root         (0)     2722 2023-02-24 12:24:40.000000 pytango-9.4.2/tango/callback.py
--rw-rw-rw-   0 root         (0) root         (0)     8009 2023-02-24 12:24:40.000000 pytango-9.4.2/tango/client.py
--rw-rw-rw-   0 root         (0) root         (0)      621 2023-02-24 12:24:40.000000 pytango-9.4.2/tango/codec.py
--rw-rw-rw-   0 root         (0) root         (0)    23142 2023-03-24 09:34:13.000000 pytango-9.4.2/tango/connection.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:21:27.752733 pytango-9.4.2/tango/databaseds/
--rw-rw-rw-   0 root         (0) root         (0)    56819 2023-02-24 12:24:40.000000 pytango-9.4.2/tango/databaseds/DataBase.xmi
--rwxrwxrwx   0 root         (0) root         (0)       88 2023-05-04 08:54:24.000000 pytango-9.4.2/tango/databaseds/DataBaseds
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-27 14:21:09.000000 pytango-9.4.2/tango/databaseds/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9052 2023-05-04 08:54:24.000000 pytango-9.4.2/tango/databaseds/create_db.sql
--rw-rw-rw-   0 root         (0) root         (0)     6116 2023-05-04 08:54:24.000000 pytango-9.4.2/tango/databaseds/create_db_tables.sql
--rw-rw-rw-   0 root         (0) root         (0)    84031 2023-05-04 08:54:24.000000 pytango-9.4.2/tango/databaseds/database.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:21:27.752733 pytango-9.4.2/tango/databaseds/db_access/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-27 14:21:09.000000 pytango-9.4.2/tango/databaseds/db_access/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    69570 2023-05-04 08:54:24.000000 pytango-9.4.2/tango/databaseds/db_access/sqlite3.py
--rw-rw-rw-   0 root         (0) root         (0)      370 2023-02-24 12:24:40.000000 pytango-9.4.2/tango/databaseds/db_errors.py
--rwxrwxrwx   0 root         (0) root         (0)     3079 2023-02-24 12:24:40.000000 pytango-9.4.2/tango/databaseds/mysql2sqlite.sh
--rw-rw-rw-   0 root         (0) root         (0)    99390 2023-02-24 12:24:40.000000 pytango-9.4.2/tango/db.py
--rw-rw-rw-   0 root         (0) root         (0)     4349 2023-05-30 07:37:03.000000 pytango-9.4.2/tango/device_attribute.py
--rw-rw-rw-   0 root         (0) root         (0)    35676 2023-02-24 12:24:40.000000 pytango-9.4.2/tango/device_class.py
--rw-rw-rw-   0 root         (0) root         (0)     2528 2023-02-24 12:24:40.000000 pytango-9.4.2/tango/device_data.py
--rw-rw-rw-   0 root         (0) root         (0)   112961 2023-07-06 14:21:46.000000 pytango-9.4.2/tango/device_proxy.py
--rw-rw-rw-   0 root         (0) root         (0)   105543 2023-07-27 08:42:45.000000 pytango-9.4.2/tango/device_server.py
--rw-rw-rw-   0 root         (0) root         (0)    24876 2023-07-11 13:40:06.000000 pytango-9.4.2/tango/encoded_attribute.py
--rw-rw-rw-   0 root         (0) root         (0)     6778 2023-02-24 12:24:40.000000 pytango-9.4.2/tango/exception.py
--rw-rw-rw-   0 root         (0) root         (0)     4377 2023-02-24 12:24:40.000000 pytango-9.4.2/tango/futures.py
--rw-rw-rw-   0 root         (0) root         (0)     1950 2023-02-24 12:24:40.000000 pytango-9.4.2/tango/futures_executor.py
--rw-rw-rw-   0 root         (0) root         (0)     4961 2023-02-24 12:24:40.000000 pytango-9.4.2/tango/gevent.py
--rw-rw-rw-   0 root         (0) root         (0)     4908 2023-02-24 12:24:40.000000 pytango-9.4.2/tango/gevent_executor.py
--rw-rw-rw-   0 root         (0) root         (0)     3186 2023-02-24 12:24:40.000000 pytango-9.4.2/tango/globals.py
--rw-rw-rw-   0 root         (0) root         (0)     6364 2023-06-30 12:46:38.000000 pytango-9.4.2/tango/green.py
--rw-rw-rw-   0 root         (0) root         (0)    30204 2023-07-06 14:21:46.000000 pytango-9.4.2/tango/group.py
--rw-rw-rw-   0 root         (0) root         (0)     3468 2023-02-24 12:24:40.000000 pytango-9.4.2/tango/group_reply.py
--rw-rw-rw-   0 root         (0) root         (0)     3192 2023-02-24 12:24:40.000000 pytango-9.4.2/tango/group_reply_list.py
--rw-rw-rw-   0 root         (0) root         (0)     9633 2023-06-23 16:56:27.000000 pytango-9.4.2/tango/log4tango.py
--rw-rw-rw-   0 root         (0) root         (0)     5396 2023-02-24 12:24:40.000000 pytango-9.4.2/tango/pipe.py
--rw-rw-rw-   0 root         (0) root         (0)     7405 2023-02-24 12:24:40.000000 pytango-9.4.2/tango/pipe_data.py
--rw-rw-rw-   0 root         (0) root         (0)     3883 2023-02-24 12:24:40.000000 pytango-9.4.2/tango/pytango_init.py
--rw-rw-rw-   0 root         (0) root         (0)     6463 2023-02-24 12:24:40.000000 pytango-9.4.2/tango/pytango_pprint.py
--rw-rw-rw-   0 root         (0) root         (0)    34307 2023-07-11 14:59:09.000000 pytango-9.4.2/tango/pyutil.py
--rw-rw-rw-   0 root         (0) root         (0)     2780 2023-07-27 08:50:35.000000 pytango-9.4.2/tango/release.py
--rw-rw-rw-   0 root         (0) root         (0)    71542 2023-07-21 16:54:44.000000 pytango-9.4.2/tango/server.py
--rw-rw-rw-   0 root         (0) root         (0)     5680 2023-02-24 12:24:40.000000 pytango-9.4.2/tango/tango_numpy.py
--rw-rw-rw-   0 root         (0) root         (0)    19382 2023-02-24 12:24:40.000000 pytango-9.4.2/tango/tango_object.py
--rw-rw-rw-   0 root         (0) root         (0)    26277 2023-07-21 16:54:44.000000 pytango-9.4.2/tango/test_context.py
--rw-rw-rw-   0 root         (0) root         (0)    11603 2023-07-06 14:21:46.000000 pytango-9.4.2/tango/test_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     5224 2023-02-24 12:24:40.000000 pytango-9.4.2/tango/time_val.py
--rw-rw-rw-   0 root         (0) root         (0)    55988 2023-07-11 13:40:06.000000 pytango-9.4.2/tango/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:21:27.753733 pytango-9.4.2/tests/
--rw-rw-rw-   0 root         (0) root         (0)     3001 2023-06-30 12:46:38.000000 pytango-9.4.2/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     1890 2023-02-24 12:24:40.000000 pytango-9.4.2/tests/test_async.py
--rw-rw-rw-   0 root         (0) root         (0)    20138 2023-07-06 14:21:46.000000 pytango-9.4.2/tests/test_client.py
--rw-rw-rw-   0 root         (0) root         (0)    10853 2023-07-27 08:42:45.000000 pytango-9.4.2/tests/test_event.py
--rw-rw-rw-   0 root         (0) root         (0)   111611 2023-07-27 12:37:05.000000 pytango-9.4.2/tests/test_server.py
--rw-rw-rw-   0 root         (0) root         (0)    18428 2023-07-21 16:54:44.000000 pytango-9.4.2/tests/test_test_context.py
--rw-rw-rw-   0 root         (0) root         (0)     2423 2023-07-21 16:54:44.000000 pytango-9.4.2/winsetup.py
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.331756 pytango-9.4.2rc1/
+-rw-r--r--   0 matveyev (30593) irc         (39)     6685 2023-06-30 12:48:12.000000 pytango-9.4.2rc1/CMakeLists.txt
+-rw-r--r--   0 matveyev (30593) irc         (39)     7883 2023-06-30 12:48:12.000000 pytango-9.4.2rc1/LICENSE.txt
+-rw-r--r--   0 matveyev (30593) irc         (39)      267 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/MANIFEST.in
+-rw-r--r--   0 matveyev (30593) irc         (39)     8584 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/Makefile
+-rw-r--r--   0 matveyev (30593) irc         (39)     6385 2023-07-13 09:38:37.331756 pytango-9.4.2rc1/PKG-INFO
+-rw-r--r--   0 matveyev (30593) irc         (39)     1560 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/PyTango.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     5027 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/README.rst
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.295756 pytango-9.4.2rc1/cmake/
+-rw-r--r--   0 matveyev (30593) irc         (39)      814 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/cmake/project_version.cc.in
+-rw-r--r--   0 matveyev (30593) irc         (39)     7407 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/cmake/project_version.cmake
+-rw-r--r--   0 matveyev (30593) irc         (39)     1672 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/cmake/project_version.h.in
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.299756 pytango-9.4.2rc1/doc/
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.299756 pytango-9.4.2rc1/doc/.devcontainer/
+-rw-r--r--   0 matveyev (30593) irc         (39)      314 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/doc/.devcontainer/Dockerfile
+-rw-r--r--   0 matveyev (30593) irc         (39)     1484 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/.devcontainer/README.md
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.307756 pytango-9.4.2rc1/doc/_static/
+-rw-r--r--   0 matveyev (30593) irc         (39)     5669 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/arrow03.png
+-rw-r--r--   0 matveyev (30593) irc         (39)   237697 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/banner1.png
+-rw-r--r--   0 matveyev (30593) irc         (39)    73015 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/banner2.png
+-rw-r--r--   0 matveyev (30593) irc         (39)    83303 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/banner3.png
+-rw-r--r--   0 matveyev (30593) irc         (39)     7419 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/doc/_static/boost_python_install.py
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.307756 pytango-9.4.2rc1/doc/_static/css/
+-rw-r--r--   0 matveyev (30593) irc         (39)   132306 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/css/tango_cs_theme.css
+-rw-r--r--   0 matveyev (30593) irc         (39)    13726 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/database.png
+-rw-r--r--   0 matveyev (30593) irc         (39)    65909 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/device.png
+-rw-r--r--   0 matveyev (30593) irc         (39)     1104 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/gallery.js
+-rw-r--r--   0 matveyev (30593) irc         (39)   603593 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/green_python.png
+-rw-r--r--   0 matveyev (30593) irc         (39)  1684994 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/green_python_original.png
+-rw-r--r--   0 matveyev (30593) irc         (39)     2765 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/ipython_db.html
+-rw-r--r--   0 matveyev (30593) irc         (39)     3829 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/ipython_motor.html
+-rw-r--r--   0 matveyev (30593) irc         (39)     3909 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/ipython_serial.html
+-rw-r--r--   0 matveyev (30593) irc         (39)    20483 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/ipython_tango.html
+-rw-r--r--   0 matveyev (30593) irc         (39)    30674 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/itango00.png
+-rw-r--r--   0 matveyev (30593) irc         (39)    14791 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/jive_powersupply.png
+-rw-r--r--   0 matveyev (30593) irc         (39)      769 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/jssor.css
+-rw-r--r--   0 matveyev (30593) irc         (39)    92207 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/jssor.js
+-rw-r--r--   0 matveyev (30593) irc         (39)   170401 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/jssor.slider.js
+-rw-r--r--   0 matveyev (30593) irc         (39)   172668 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/logo-medium.png
+-rwxr-xr-x   0 matveyev (30593) irc         (39)     4030 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/logo.ico
+-rw-r--r--   0 matveyev (30593) irc         (39)    99573 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/logo.png
+-rw-r--r--   0 matveyev (30593) irc         (39)   221457 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/mocking-tango-db-access-crossed-out.png
+-rw-r--r--   0 matveyev (30593) irc         (39)   145562 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/mocking-tango-db-access.png
+-rw-r--r--   0 matveyev (30593) irc         (39)    63184 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/mocking-tango-test-case-not-mocked.png
+-rw-r--r--   0 matveyev (30593) irc         (39)    54671 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/mocking-tango-test-case-real-vs-mocked.png
+-rw-r--r--   0 matveyev (30593) irc         (39)   179107 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/mocking-tango-test-doubles.png
+-rw-r--r--   0 matveyev (30593) irc         (39)    13299 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/motor.png
+-rw-r--r--   0 matveyev (30593) irc         (39)     2455 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/doc/_static/power_supply.py
+-rw-r--r--   0 matveyev (30593) irc         (39)      891 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/project-config.jam
+-rw-r--r--   0 matveyev (30593) irc         (39)     6201 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/pytango.css
+-rw-r--r--   0 matveyev (30593) irc         (39)     6323 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/serial.png
+-rw-r--r--   0 matveyev (30593) irc         (39)      720 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/slideshow.js
+-rw-r--r--   0 matveyev (30593) irc         (39)    15763 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/starter.png
+-rw-r--r--   0 matveyev (30593) irc         (39)   171117 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/testing-approaches-device-test-context-x2.png
+-rw-r--r--   0 matveyev (30593) irc         (39)   211964 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/testing-approaches-device-test-context.png
+-rw-r--r--   0 matveyev (30593) irc         (39)   206869 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/testing-approaches-hybrid.png
+-rw-r--r--   0 matveyev (30593) irc         (39)   336790 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/testing-approaches-multi-device-test-context.png
+-rw-r--r--   0 matveyev (30593) irc         (39)   108016 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_static/testing-approaches-real-facility.png
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.307756 pytango-9.4.2rc1/doc/_templates/
+-rw-r--r--   0 matveyev (30593) irc         (39)      695 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/_templates/breadcrumbs.html
+-rw-r--r--   0 matveyev (30593) irc         (39)    14238 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/doc/_templates/index.html
+-rw-r--r--   0 matveyev (30593) irc         (39)      642 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/doc/_templates/indexsidebar.html
+-rw-r--r--   0 matveyev (30593) irc         (39)      246 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/api.rst
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.307756 pytango-9.4.2rc1/doc/client_api/
+-rw-r--r--   0 matveyev (30593) irc         (39)      111 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/client_api/attribute_proxy.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)      187 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/doc/client_api/device_proxy.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)      474 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/doc/client_api/green.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)     1157 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/client_api/group.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)      139 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/client_api/index.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)     2410 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/client_api/miscellaneous.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)     1056 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/client_api/other.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)    18665 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/doc/conf.py
+-rw-r--r--   0 matveyev (30593) irc         (39)      423 2023-06-30 12:48:12.000000 pytango-9.4.2rc1/doc/contents.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)    42078 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/data_types.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)      493 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/database.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)      171 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/encoded.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)      120 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/doc/environment.yml
+-rw-r--r--   0 matveyev (30593) irc         (39)    12704 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/exception.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)     1508 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/faq.rst
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.307756 pytango-9.4.2rc1/doc/green_modes/
+-rw-r--r--   0 matveyev (30593) irc         (39)      525 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/green_modes/client_asyncio_mode.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)     3542 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/green_modes/client_futures_mode.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)     4036 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/green_modes/client_gevent_mode.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)     1220 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/green_modes/green.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)     1204 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/green_modes/green_modes_client.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)     2473 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/green_modes/green_modes_server.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)     9922 2023-07-11 14:09:19.000000 pytango-9.4.2rc1/doc/how-to-contribute.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)    62310 2023-07-11 14:09:19.000000 pytango-9.4.2rc1/doc/howto.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)       61 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/indexes.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)      524 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/itango.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)   206038 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/logo-medium.bmp
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.307756 pytango-9.4.2rc1/doc/man/
+-rw-r--r--   0 matveyev (30593) irc         (39)      451 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/man/itango.1
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.307756 pytango-9.4.2rc1/doc/migration/
+-rw-r--r--   0 matveyev (30593) irc         (39)      212 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/doc/migration/index.rst
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.307756 pytango-9.4.2rc1/doc/migration/to-9.4/
+-rw-r--r--   0 matveyev (30593) irc         (39)     1566 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/doc/migration/to-9.4/attr-decorators.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)     1156 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/doc/migration/to-9.4/deps-install.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)    16392 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/doc/migration/to-9.4/empty-attrs.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)     2033 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/doc/migration/to-9.4/extract-as.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)     2075 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/doc/migration/to-9.4/hl-dev-enum.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)      756 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/doc/migration/to-9.4/hl-dynamic.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)      377 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/doc/migration/to-9.4/index.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)     1344 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/doc/migration/to-9.4/logging-percent-sym.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)     3887 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/doc/migration/to-9.4/non-bound-user-funcs.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)     1997 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/doc/migration/to-9.4/optional-proxy-attrs.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)     5186 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/doc/mock_tango_extension.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     8020 2023-07-12 14:38:10.000000 pytango-9.4.2rc1/doc/news.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)     9178 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/doc/quicktour.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)   170620 2023-07-12 14:38:10.000000 pytango-9.4.2rc1/doc/revision.rst
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.307756 pytango-9.4.2rc1/doc/server_api/
+-rw-r--r--   0 matveyev (30593) irc         (39)      434 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/server_api/attribute.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)      141 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/server_api/device.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)       98 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/server_api/device_class.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)      158 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/server_api/index.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)      419 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/server_api/logging.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)    10620 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/server_api/server.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)      101 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/server_api/util.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)     6458 2023-07-12 14:38:10.000000 pytango-9.4.2rc1/doc/start.rst
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.311756 pytango-9.4.2rc1/doc/tep/
+-rw-r--r--   0 matveyev (30593) irc         (39)    56811 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/tep/DataBase.xmi
+-rw-r--r--   0 matveyev (30593) irc         (39)   100867 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/doc/tep/database.py
+-rw-r--r--   0 matveyev (30593) irc         (39)    19326 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/tep/tep-0001.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)    17205 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/tep/tep-0002.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)      222 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/tep.rst
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.311756 pytango-9.4.2rc1/doc/testing/
+-rw-r--r--   0 matveyev (30593) irc         (39)     3725 2023-07-11 14:09:19.000000 pytango-9.4.2rc1/doc/testing/coverage.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)     8724 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/testing/mocks.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)      643 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/testing/test_context.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)    15469 2023-07-11 14:09:19.000000 pytango-9.4.2rc1/doc/testing/testing_approaches.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)      276 2023-07-11 14:09:19.000000 pytango-9.4.2rc1/doc/testing.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)     1088 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/utilities.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)     2400 2023-06-30 12:48:12.000000 pytango-9.4.2rc1/doc/version-policy.rst
+-rw-r--r--   0 matveyev (30593) irc         (39)     6737 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/doc/windows_notes.txt
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.291756 pytango-9.4.2rc1/examples/
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.311756 pytango-9.4.2rc1/examples/Clock/
+-rw-r--r--   0 matveyev (30593) irc         (39)      315 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/Clock/Clock.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     1867 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/Clock/ClockDS.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     1490 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/Clock/client.py
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.311756 pytango-9.4.2rc1/examples/TuringMachine/
+-rw-r--r--   0 matveyev (30593) irc         (39)     2062 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/TuringMachine/TuringMachine.py
+-rw-r--r--   0 matveyev (30593) irc         (39)      447 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/TuringMachine/turing_client.py
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.311756 pytango-9.4.2rc1/examples/asyncio_green_mode/
+-rw-r--r--   0 matveyev (30593) irc         (39)       38 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/asyncio_green_mode/__init__.py
+-rw-r--r--   0 matveyev (30593) irc         (39)      969 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/asyncio_green_mode/asyncio_device_example.py
+-rw-r--r--   0 matveyev (30593) irc         (39)      281 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/asyncio_green_mode/asyncio_simple_example.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     1886 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/asyncio_green_mode/tcp_server_example.py
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.311756 pytango-9.4.2rc1/examples/dynamic/
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.311756 pytango-9.4.2rc1/examples/dynamic/common/
+-rw-r--r--   0 matveyev (30593) irc         (39)        0 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/dynamic/common/__init__.py
+-rw-r--r--   0 matveyev (30593) irc         (39)      285 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/dynamic/common/roi.py
+-rw-r--r--   0 matveyev (30593) irc         (39)      638 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/dynamic/dynamic_client.py
+-rw-r--r--   0 matveyev (30593) irc         (39)      958 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/dynamic/dynamic_server.py
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.311756 pytango-9.4.2rc1/examples/fwdAttr/
+-rw-r--r--   0 matveyev (30593) irc         (39)      883 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/fwdAttr/FwdServer.py
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.311756 pytango-9.4.2rc1/examples/interfacechangeEvents/
+-rw-r--r--   0 matveyev (30593) irc         (39)     1954 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/interfacechangeEvents/ClassFactory.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     1841 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/interfacechangeEvents/IfchangeClient.py
+-rw-r--r--   0 matveyev (30593) irc         (39)    11392 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/interfacechangeEvents/IfchangeServer.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     5744 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/interfacechangeEvents/IfchangeServer.h
+-rw-r--r--   0 matveyev (30593) irc         (39)     1926 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/interfacechangeEvents/IfchangeServer.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     4643 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/interfacechangeEvents/IfchangeServer.xmi
+-rw-r--r--   0 matveyev (30593) irc         (39)    21544 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/interfacechangeEvents/IfchangeServerClass.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     7254 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/interfacechangeEvents/IfchangeServerClass.h
+-rw-r--r--   0 matveyev (30593) irc         (39)     6341 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/interfacechangeEvents/IfchangeServerDynAttrUtils.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     5037 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/interfacechangeEvents/IfchangeServerStateMachine.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     5095 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/interfacechangeEvents/Makefile
+-rw-r--r--   0 matveyev (30593) irc         (39)     5095 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/interfacechangeEvents/Makefile.bck
+-rw-r--r--   0 matveyev (30593) irc         (39)     2731 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/interfacechangeEvents/main.cpp
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.311756 pytango-9.4.2rc1/examples/mandatory/
+-rw-r--r--   0 matveyev (30593) irc         (39)      576 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/mandatory/MandatoryPropertyServer.py
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.311756 pytango-9.4.2rc1/examples/many/
+-rw-r--r--   0 matveyev (30593) irc         (39)      388 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/many/many_client.py
+-rw-r--r--   0 matveyev (30593) irc         (39)      685 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/many/many_server.py
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.311756 pytango-9.4.2rc1/examples/multi/
+-rw-r--r--   0 matveyev (30593) irc         (39)      700 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/multi/multi_client.py
+-rw-r--r--   0 matveyev (30593) irc         (39)      955 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/multi/multi_server.py
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.311756 pytango-9.4.2rc1/examples/multidevicetestcontext/
+-rw-r--r--   0 matveyev (30593) irc         (39)      960 2023-07-11 12:35:26.000000 pytango-9.4.2rc1/examples/multidevicetestcontext/conftest.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     2763 2023-07-11 12:35:26.000000 pytango-9.4.2rc1/examples/multidevicetestcontext/test_integration.py
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.311756 pytango-9.4.2rc1/examples/pipeEvents/
+-rw-r--r--   0 matveyev (30593) irc         (39)     1926 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/pipeEvents/ClassFactory.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     5047 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/pipeEvents/Makefile
+-rw-r--r--   0 matveyev (30593) irc         (39)     1579 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/pipeEvents/PipeEventClient.py
+-rw-r--r--   0 matveyev (30593) irc         (39)    15129 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/pipeEvents/PipeServer.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     4833 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/pipeEvents/PipeServer.h
+-rw-r--r--   0 matveyev (30593) irc         (39)     2977 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/pipeEvents/PipeServer.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     2512 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/pipeEvents/PipeServer.xmi
+-rw-r--r--   0 matveyev (30593) irc         (39)    19277 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/pipeEvents/PipeServerClass.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     5100 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/pipeEvents/PipeServerClass.h
+-rw-r--r--   0 matveyev (30593) irc         (39)     3687 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/pipeEvents/PipeServerStateMachine.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     2719 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/pipeEvents/main.cpp
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.315756 pytango-9.4.2rc1/examples/pipes/
+-rw-r--r--   0 matveyev (30593) irc         (39)     1926 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/pipes/ClassFactory.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     5047 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/pipes/Makefile
+-rw-r--r--   0 matveyev (30593) irc         (39)      893 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/pipes/PipeClient.py
+-rw-r--r--   0 matveyev (30593) irc         (39)    11859 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/pipes/PipeServer.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     4416 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/pipes/PipeServer.h
+-rw-r--r--   0 matveyev (30593) irc         (39)     1031 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/pipes/PipeServer.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     2089 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/pipes/PipeServer.xmi
+-rw-r--r--   0 matveyev (30593) irc         (39)    18280 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/pipes/PipeServerClass.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     4186 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/pipes/PipeServerClass.h
+-rw-r--r--   0 matveyev (30593) irc         (39)     3082 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/pipes/PipeServerStateMachine.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)        0 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/pipes/__init__.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     2719 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/pipes/main.cpp
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.315756 pytango-9.4.2rc1/examples/simple/
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.315756 pytango-9.4.2rc1/examples/simple/common/
+-rw-r--r--   0 matveyev (30593) irc         (39)        0 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/simple/common/__init__.py
+-rw-r--r--   0 matveyev (30593) irc         (39)      285 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/simple/common/roi.py
+-rw-r--r--   0 matveyev (30593) irc         (39)      638 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/simple/simple_client.py
+-rw-r--r--   0 matveyev (30593) irc         (39)      963 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/simple/simple_server.py
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.315756 pytango-9.4.2rc1/examples/training/
+-rw-r--r--   0 matveyev (30593) irc         (39)     5106 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/training/README.md
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.315756 pytango-9.4.2rc1/examples/training/client/
+-rwxr-xr-x   0 matveyev (30593) irc         (39)     1784 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/training/client/command01.py
+-rwxr-xr-x   0 matveyev (30593) irc         (39)     1815 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/training/client/command02.py
+-rwxr-xr-x   0 matveyev (30593) irc         (39)     1185 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/training/client/reading01.py
+-rwxr-xr-x   0 matveyev (30593) irc         (39)     1636 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/training/client/reading02.py
+-rwxr-xr-x   0 matveyev (30593) irc         (39)     5644 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/training/client/reading03.py
+-rwxr-xr-x   0 matveyev (30593) irc         (39)     1251 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/training/client/writing01.py
+-rwxr-xr-x   0 matveyev (30593) irc         (39)     1260 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/training/client/writing02.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     2444 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/training/docker-compose.yml
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.315756 pytango-9.4.2rc1/examples/training/server/
+-rwxr-xr-x   0 matveyev (30593) irc         (39)      412 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/training/server/high-level-api.py
+-rwxr-xr-x   0 matveyev (30593) irc         (39)     1331 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/training/server/libps.py
+-rwxr-xr-x   0 matveyev (30593) irc         (39)     1340 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/training/server/low-level-api.py
+-rwxr-xr-x   0 matveyev (30593) irc         (39)     3831 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/training/server/ps-simulator.py
+-rwxr-xr-x   0 matveyev (30593) irc         (39)      394 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/training/server/ps0a.py
+-rwxr-xr-x   0 matveyev (30593) irc         (39)     1058 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/training/server/ps0b-push-event.py
+-rwxr-xr-x   0 matveyev (30593) irc         (39)      623 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/training/server/ps0b.py
+-rwxr-xr-x   0 matveyev (30593) irc         (39)     1216 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/training/server/ps0c.py
+-rwxr-xr-x   0 matveyev (30593) irc         (39)     1217 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/training/server/ps1-gevent.py
+-rwxr-xr-x   0 matveyev (30593) irc         (39)     1154 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/training/server/ps1-use-lib-logging.py
+-rwxr-xr-x   0 matveyev (30593) irc         (39)      943 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/training/server/ps1-use-lib.py
+-rwxr-xr-x   0 matveyev (30593) irc         (39)     1119 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/training/server/ps1.py
+-rwxr-xr-x   0 matveyev (30593) irc         (39)     1770 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/training/server/ps2-gevent-check.py
+-rwxr-xr-x   0 matveyev (30593) irc         (39)     1462 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/training/server/ps2-gevent.py
+-rw-r--r--   0 matveyev (30593) irc         (39)      351 2023-03-14 11:21:37.000000 pytango-9.4.2rc1/examples/training/server/test_ps0a.py
+-rw-r--r--   0 matveyev (30593) irc         (39)      929 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/training/server/test_ps0b.py
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.315756 pytango-9.4.2rc1/examples/training/webinars/
+-rw-r--r--   0 matveyev (30593) irc         (39)      648 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/training/webinars/crash_example.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     3557 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/examples/training/webinars/test_webinar.py
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.323756 pytango-9.4.2rc1/ext/
+-rw-r--r--   0 matveyev (30593) irc         (39)     2498 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/api_util.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     1102 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/archive_event_info.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     2618 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/attr_conf_event_data.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     1299 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/attribute_alarm_info.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)      872 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/attribute_dimension.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)      989 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/attribute_event_info.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)      921 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/attribute_info.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     1276 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/attribute_info_ex.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     4095 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/attribute_proxy.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)    16584 2023-06-30 12:48:12.000000 pytango-9.4.2rc1/ext/base_types.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     3388 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/base_types_numpy.hpp
+-rw-r--r--   0 matveyev (30593) irc         (39)    15060 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/ext/callback.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     4682 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/callback.h
+-rw-r--r--   0 matveyev (30593) irc         (39)      981 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/change_event_info.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)      824 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/command_info.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     5786 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/connection.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)    18026 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/constants.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     2842 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/data_ready_event_data.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)    19287 2023-06-22 12:57:49.000000 pytango-9.4.2rc1/ext/database.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     4296 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/db.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     1228 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/ext/defs.h
+-rw-r--r--   0 matveyev (30593) irc         (39)     1321 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/dev_command_info.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     2172 2023-06-30 12:48:12.000000 pytango-9.4.2rc1/ext/dev_error.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)    33447 2023-06-30 12:48:12.000000 pytango-9.4.2rc1/ext/device_attribute.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     7614 2023-06-30 12:48:12.000000 pytango-9.4.2rc1/ext/device_attribute.h
+-rw-r--r--   0 matveyev (30593) irc         (39)    13598 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/device_attribute.h.gch
+-rw-r--r--   0 matveyev (30593) irc         (39)     2667 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/device_attribute_config.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     1013 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/device_attribute_history.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)    10170 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/device_attribute_numpy.hpp
+-rw-r--r--   0 matveyev (30593) irc         (39)  1831316 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/device_attribute_numpy.hpp.gch
+-rw-r--r--   0 matveyev (30593) irc         (39)     8332 2023-06-30 12:48:12.000000 pytango-9.4.2rc1/ext/device_data.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     1185 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/device_data_history.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     1120 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/device_info.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)    14245 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/device_pipe.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     1743 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/device_pipe.h
+-rw-r--r--   0 matveyev (30593) irc         (39)    42737 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/device_proxy.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     2898 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/devintr_change_event_data.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)    12739 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/enums.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     2951 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/event_data.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)    18550 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/exception.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     3594 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/exception.h
+-rw-r--r--   0 matveyev (30593) irc         (39)    18306 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/fast_from_py.h
+-rw-r--r--   0 matveyev (30593) irc         (39)     9248 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/fast_from_py_numpy.hpp
+-rw-r--r--   0 matveyev (30593) irc         (39)    16044 2023-06-30 12:48:12.000000 pytango-9.4.2rc1/ext/from_py.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)    26882 2023-06-30 12:48:12.000000 pytango-9.4.2rc1/ext/from_py.h
+-rw-r--r--   0 matveyev (30593) irc         (39)    13470 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/group.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     2717 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/group_reply.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     1971 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/group_reply_list.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     1204 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/locker_info.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)      725 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/locking_thread.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)      909 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/periodic_event_info.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     2503 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/pipe_event_data.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     1151 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/pipe_info.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     1047 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/poll_device.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)      577 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/precompiled_header.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     1307 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/precompiled_header.hpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     3343 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/pytango.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)      652 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/pytgutils.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     2021 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/pytgutils.h
+-rw-r--r--   0 matveyev (30593) irc         (39)     8373 2023-06-30 12:48:12.000000 pytango-9.4.2rc1/ext/pyutils.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     7427 2023-06-30 12:48:12.000000 pytango-9.4.2rc1/ext/pyutils.h
+-rw-r--r--   0 matveyev (30593) irc         (39)    13598 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/pyutils.h.gch
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.323756 pytango-9.4.2rc1/ext/server/
+-rw-r--r--   0 matveyev (30593) irc         (39)    10787 2023-07-05 13:49:12.000000 pytango-9.4.2rc1/ext/server/attr.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)    10786 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/server/attr.h
+-rw-r--r--   0 matveyev (30593) irc         (39)    34005 2023-06-30 12:48:12.000000 pytango-9.4.2rc1/ext/server/attribute.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     2860 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/server/attribute.h
+-rw-r--r--   0 matveyev (30593) irc         (39)     3350 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/server/auto_monitor.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)    10091 2023-06-30 12:48:12.000000 pytango-9.4.2rc1/ext/server/command.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     1665 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/server/command.h
+-rw-r--r--   0 matveyev (30593) irc         (39)    15118 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/server/device_class.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     6475 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/server/device_class.h
+-rw-r--r--   0 matveyev (30593) irc         (39)    67588 2023-07-11 14:09:19.000000 pytango-9.4.2rc1/ext/server/device_impl.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)    13502 2023-07-11 14:09:19.000000 pytango-9.4.2rc1/ext/server/device_impl.h
+-rw-r--r--   0 matveyev (30593) irc         (39)     7705 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/server/dserver.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)    46343 2023-07-12 14:38:10.000000 pytango-9.4.2rc1/ext/server/encoded_attribute.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     1084 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/server/fwdAttr.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     6352 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/server/log4tango.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     2367 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/server/multi_attribute.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     1190 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/server/multi_class_attribute.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)    19095 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/server/pipe.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     2568 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/server/pipe.h
+-rw-r--r--   0 matveyev (30593) irc         (39)     1904 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/server/subdev.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)    11368 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/server/tango_util.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     4608 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/server/user_default_attr_prop.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)      911 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/server/user_default_pipe_prop.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)    23854 2023-07-11 14:09:19.000000 pytango-9.4.2rc1/ext/server/wattribute.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     2575 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/server/wattribute_numpy.hpp
+-rw-r--r--   0 matveyev (30593) irc         (39)     3003 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/tango_numpy.h
+-rw-r--r--   0 matveyev (30593) irc         (39)    24364 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/tgutils.h
+-rw-r--r--   0 matveyev (30593) irc         (39)      885 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/time_val.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)    12585 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/to_py.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)    12370 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/to_py.h
+-rw-r--r--   0 matveyev (30593) irc         (39)     5383 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/to_py_numpy.hpp
+-rw-r--r--   0 matveyev (30593) irc         (39)      723 2023-03-14 11:21:25.000000 pytango-9.4.2rc1/ext/version.cpp
+-rw-r--r--   0 matveyev (30593) irc         (39)      554 2023-03-14 11:21:39.000000 pytango-9.4.2rc1/pyproject.toml
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.327756 pytango-9.4.2rc1/pytango.egg-info/
+-rw-r--r--   0 matveyev (30593) irc         (39)     6385 2023-07-13 09:38:37.000000 pytango-9.4.2rc1/pytango.egg-info/PKG-INFO
+-rw-r--r--   0 matveyev (30593) irc         (39)    13372 2023-07-13 09:38:37.000000 pytango-9.4.2rc1/pytango.egg-info/SOURCES.txt
+-rw-r--r--   0 matveyev (30593) irc         (39)        1 2023-07-13 09:38:37.000000 pytango-9.4.2rc1/pytango.egg-info/dependency_links.txt
+-rw-r--r--   0 matveyev (30593) irc         (39)       95 2023-07-13 09:38:37.000000 pytango-9.4.2rc1/pytango.egg-info/requires.txt
+-rw-r--r--   0 matveyev (30593) irc         (39)       21 2023-07-13 09:38:37.000000 pytango-9.4.2rc1/pytango.egg-info/top_level.txt
+-rw-r--r--   0 matveyev (30593) irc         (39)      241 2023-07-13 09:38:37.331756 pytango-9.4.2rc1/setup.cfg
+-rw-r--r--   0 matveyev (30593) irc         (39)    15707 2023-07-11 12:35:26.000000 pytango-9.4.2rc1/setup.py
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.327756 pytango-9.4.2rc1/tango/
+-rw-r--r--   0 matveyev (30593) irc         (39)    10466 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tango/__init__.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     5184 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tango/api_util.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     4464 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tango/asyncio.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     4016 2023-06-30 12:48:12.000000 pytango-9.4.2rc1/tango/asyncio_executor.py
+-rw-r--r--   0 matveyev (30593) irc         (39)    15383 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tango/attr_data.py
+-rw-r--r--   0 matveyev (30593) irc         (39)    18234 2023-07-11 12:35:26.000000 pytango-9.4.2rc1/tango/attribute_proxy.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     2092 2023-03-14 11:21:38.000000 pytango-9.4.2rc1/tango/auto_monitor.py
+-rw-r--r--   0 matveyev (30593) irc         (39)    29926 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tango/base_types.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     2722 2023-03-14 11:21:38.000000 pytango-9.4.2rc1/tango/callback.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     8009 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tango/client.py
+-rw-r--r--   0 matveyev (30593) irc         (39)      621 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tango/codec.py
+-rw-r--r--   0 matveyev (30593) irc         (39)    23142 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tango/connection.py
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.331756 pytango-9.4.2rc1/tango/databaseds/
+-rw-r--r--   0 matveyev (30593) irc         (39)    56819 2023-03-14 11:21:38.000000 pytango-9.4.2rc1/tango/databaseds/DataBase.xmi
+-rwxr-xr-x   0 matveyev (30593) irc         (39)       88 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tango/databaseds/DataBaseds
+-rw-r--r--   0 matveyev (30593) irc         (39)        0 2023-03-14 11:21:38.000000 pytango-9.4.2rc1/tango/databaseds/__init__.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     9052 2023-03-14 11:21:38.000000 pytango-9.4.2rc1/tango/databaseds/create_db.sql
+-rw-r--r--   0 matveyev (30593) irc         (39)     6116 2023-03-14 11:21:38.000000 pytango-9.4.2rc1/tango/databaseds/create_db_tables.sql
+-rw-r--r--   0 matveyev (30593) irc         (39)    84031 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tango/databaseds/database.py
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.331756 pytango-9.4.2rc1/tango/databaseds/db_access/
+-rw-r--r--   0 matveyev (30593) irc         (39)        0 2023-03-14 11:21:38.000000 pytango-9.4.2rc1/tango/databaseds/db_access/__init__.py
+-rw-r--r--   0 matveyev (30593) irc         (39)    69570 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tango/databaseds/db_access/sqlite3.py
+-rw-r--r--   0 matveyev (30593) irc         (39)      370 2023-03-14 11:21:38.000000 pytango-9.4.2rc1/tango/databaseds/db_errors.py
+-rwxr-xr-x   0 matveyev (30593) irc         (39)     3079 2023-03-14 11:21:38.000000 pytango-9.4.2rc1/tango/databaseds/mysql2sqlite.sh
+-rw-r--r--   0 matveyev (30593) irc         (39)    99390 2023-06-22 12:57:49.000000 pytango-9.4.2rc1/tango/db.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     4349 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tango/device_attribute.py
+-rw-r--r--   0 matveyev (30593) irc         (39)    35676 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tango/device_class.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     2528 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tango/device_data.py
+-rw-r--r--   0 matveyev (30593) irc         (39)   112961 2023-07-11 12:35:26.000000 pytango-9.4.2rc1/tango/device_proxy.py
+-rw-r--r--   0 matveyev (30593) irc         (39)   105543 2023-07-11 14:09:19.000000 pytango-9.4.2rc1/tango/device_server.py
+-rw-r--r--   0 matveyev (30593) irc         (39)    24876 2023-07-11 13:23:50.000000 pytango-9.4.2rc1/tango/encoded_attribute.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     6778 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tango/exception.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     4377 2023-03-14 11:21:38.000000 pytango-9.4.2rc1/tango/futures.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     1950 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tango/futures_executor.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     4961 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tango/gevent.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     4908 2023-06-19 08:20:41.000000 pytango-9.4.2rc1/tango/gevent_executor.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     3186 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tango/globals.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     6364 2023-06-30 12:48:12.000000 pytango-9.4.2rc1/tango/green.py
+-rw-r--r--   0 matveyev (30593) irc         (39)    30204 2023-07-11 12:35:26.000000 pytango-9.4.2rc1/tango/group.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     3468 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tango/group_reply.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     3192 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tango/group_reply_list.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     9633 2023-07-05 13:49:23.000000 pytango-9.4.2rc1/tango/log4tango.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     5396 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tango/pipe.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     7405 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tango/pipe_data.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     3883 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tango/pytango_init.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     6463 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tango/pytango_pprint.py
+-rw-r--r--   0 matveyev (30593) irc         (39)    34307 2023-07-11 14:09:19.000000 pytango-9.4.2rc1/tango/pyutil.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     2789 2023-07-13 09:20:11.000000 pytango-9.4.2rc1/tango/release.py
+-rw-r--r--   0 matveyev (30593) irc         (39)    71542 2023-07-11 14:09:19.000000 pytango-9.4.2rc1/tango/server.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     5680 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tango/tango_numpy.py
+-rw-r--r--   0 matveyev (30593) irc         (39)    19382 2023-06-19 08:20:41.000000 pytango-9.4.2rc1/tango/tango_object.py
+-rw-r--r--   0 matveyev (30593) irc         (39)    26277 2023-07-11 14:09:19.000000 pytango-9.4.2rc1/tango/test_context.py
+-rw-r--r--   0 matveyev (30593) irc         (39)    11603 2023-07-11 12:35:26.000000 pytango-9.4.2rc1/tango/test_utils.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     5224 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tango/time_val.py
+-rw-r--r--   0 matveyev (30593) irc         (39)    55988 2023-07-11 13:23:50.000000 pytango-9.4.2rc1/tango/utils.py
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-07-13 09:38:37.331756 pytango-9.4.2rc1/tests/
+-rw-r--r--   0 matveyev (30593) irc         (39)     3001 2023-06-30 12:48:12.000000 pytango-9.4.2rc1/tests/conftest.py
+-rw-r--r--   0 matveyev (30593) irc         (39)      209 2023-07-05 14:13:23.000000 pytango-9.4.2rc1/tests/report.xml
+-rw-r--r--   0 matveyev (30593) irc         (39)     1890 2023-06-19 08:02:11.000000 pytango-9.4.2rc1/tests/test_async.py
+-rw-r--r--   0 matveyev (30593) irc         (39)    20138 2023-07-11 12:35:26.000000 pytango-9.4.2rc1/tests/test_client.py
+-rw-r--r--   0 matveyev (30593) irc         (39)    10853 2023-06-19 08:03:31.000000 pytango-9.4.2rc1/tests/test_event.py
+-rw-r--r--   0 matveyev (30593) irc         (39)   111640 2023-07-12 14:38:10.000000 pytango-9.4.2rc1/tests/test_server.py
+-rw-r--r--   0 matveyev (30593) irc         (39)    18428 2023-07-11 14:09:19.000000 pytango-9.4.2rc1/tests/test_test_context.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     2423 2023-06-30 12:48:12.000000 pytango-9.4.2rc1/winsetup.py
```

### Comparing `pytango-9.4.2/CMakeLists.txt` & `pytango-9.4.2rc1/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/LICENSE.txt` & `pytango-9.4.2rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/Makefile` & `pytango-9.4.2rc1/Makefile`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/PKG-INFO` & `pytango-9.4.2rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pytango
-Version: 9.4.2
+Version: 9.4.2rc1
 Summary: A python binding for the Tango control system
 Home-page: http://gitlab.com/tango-controls/pytango
+Download-URL: http://pypi.python.org/pypi/pytango
 Author: Tiago Coutinho
 Author-email: coutinho@esrf.fr
 License: LGPL
-Download-URL: http://pypi.python.org/pypi/pytango
 Keywords: Tango,CORBA,binding
 Platform: Linux
 Platform: Windows XP/Vista/7/8/10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
@@ -185,8 +185,7 @@
 .. _IPython: http://ipython.org
 
 .. _documentation: http://pytango.readthedocs.io/en/latest
 .. _Tango forums: http://tango-controls.org/community/forum
 .. _PR and bug reports: PyTango_
 .. _sources: PyTango_
 .. _How to Contribute: http://pytango.readthedocs.io/en/latest/how-to-contribute.html#how-to-contribute
-
```

### Comparing `pytango-9.4.2/PyTango.py` & `pytango-9.4.2rc1/PyTango.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/README.rst` & `pytango-9.4.2rc1/README.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/cmake/project_version.cc.in` & `pytango-9.4.2rc1/cmake/project_version.cc.in`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/cmake/project_version.cmake` & `pytango-9.4.2rc1/cmake/project_version.cmake`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/cmake/project_version.h.in` & `pytango-9.4.2rc1/cmake/project_version.h.in`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/.devcontainer/README.md` & `pytango-9.4.2rc1/doc/.devcontainer/README.md`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/_static/arrow03.png` & `pytango-9.4.2rc1/doc/_static/arrow03.png`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/_static/banner1.png` & `pytango-9.4.2rc1/doc/_static/banner1.png`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/_static/banner2.png` & `pytango-9.4.2rc1/doc/_static/banner2.png`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/_static/banner3.png` & `pytango-9.4.2rc1/doc/_static/banner3.png`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/_static/boost_python_install.py` & `pytango-9.4.2rc1/doc/_static/boost_python_install.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/_static/css/tango_cs_theme.css` & `pytango-9.4.2rc1/doc/_static/css/tango_cs_theme.css`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/_static/database.png` & `pytango-9.4.2rc1/doc/_static/database.png`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/_static/device.png` & `pytango-9.4.2rc1/doc/_static/device.png`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/_static/gallery.js` & `pytango-9.4.2rc1/doc/_static/gallery.js`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/_static/green_python.png` & `pytango-9.4.2rc1/doc/_static/green_python.png`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/_static/green_python_original.png` & `pytango-9.4.2rc1/doc/_static/green_python_original.png`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/_static/ipython_db.html` & `pytango-9.4.2rc1/doc/_static/ipython_db.html`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/_static/ipython_motor.html` & `pytango-9.4.2rc1/doc/_static/ipython_motor.html`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/_static/ipython_serial.html` & `pytango-9.4.2rc1/doc/_static/ipython_serial.html`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/_static/ipython_tango.html` & `pytango-9.4.2rc1/doc/_static/ipython_tango.html`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/_static/itango00.png` & `pytango-9.4.2rc1/doc/_static/itango00.png`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/_static/jive_powersupply.png` & `pytango-9.4.2rc1/doc/_static/jive_powersupply.png`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/_static/jssor.css` & `pytango-9.4.2rc1/doc/_static/jssor.css`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/_static/jssor.js` & `pytango-9.4.2rc1/doc/_static/jssor.js`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/_static/jssor.slider.js` & `pytango-9.4.2rc1/doc/_static/jssor.slider.js`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/_static/logo-medium.png` & `pytango-9.4.2rc1/doc/_static/logo-medium.png`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/_static/logo.ico` & `pytango-9.4.2rc1/doc/_static/logo.ico`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/_static/logo.png` & `pytango-9.4.2rc1/doc/_static/logo.png`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/_static/mocking-tango-db-access-crossed-out.png` & `pytango-9.4.2rc1/doc/_static/mocking-tango-db-access-crossed-out.png`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/_static/mocking-tango-db-access.png` & `pytango-9.4.2rc1/doc/_static/mocking-tango-db-access.png`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/_static/mocking-tango-test-case-not-mocked.png` & `pytango-9.4.2rc1/doc/_static/mocking-tango-test-case-not-mocked.png`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/_static/mocking-tango-test-case-real-vs-mocked.png` & `pytango-9.4.2rc1/doc/_static/mocking-tango-test-case-real-vs-mocked.png`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/_static/mocking-tango-test-doubles.png` & `pytango-9.4.2rc1/doc/_static/mocking-tango-test-doubles.png`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/_static/motor.png` & `pytango-9.4.2rc1/doc/_static/motor.png`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/_static/power_supply.py` & `pytango-9.4.2rc1/doc/_static/power_supply.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/_static/project-config.jam` & `pytango-9.4.2rc1/doc/_static/project-config.jam`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/_static/pytango.css` & `pytango-9.4.2rc1/doc/_static/pytango.css`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/_static/serial.png` & `pytango-9.4.2rc1/doc/_static/serial.png`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/_static/slideshow.js` & `pytango-9.4.2rc1/doc/_static/slideshow.js`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/_static/starter.png` & `pytango-9.4.2rc1/doc/_static/starter.png`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/_static/testing-approaches-device-test-context-x2.png` & `pytango-9.4.2rc1/doc/_static/testing-approaches-device-test-context-x2.png`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/_static/testing-approaches-device-test-context.png` & `pytango-9.4.2rc1/doc/_static/testing-approaches-device-test-context.png`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/_static/testing-approaches-hybrid.png` & `pytango-9.4.2rc1/doc/_static/testing-approaches-hybrid.png`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/_static/testing-approaches-multi-device-test-context.png` & `pytango-9.4.2rc1/doc/_static/testing-approaches-multi-device-test-context.png`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/_static/testing-approaches-real-facility.png` & `pytango-9.4.2rc1/doc/_static/testing-approaches-real-facility.png`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/_templates/breadcrumbs.html` & `pytango-9.4.2rc1/doc/_templates/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/_templates/index.html` & `pytango-9.4.2rc1/doc/_templates/index.html`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/_templates/indexsidebar.html` & `pytango-9.4.2rc1/doc/_templates/indexsidebar.html`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/client_api/group.rst` & `pytango-9.4.2rc1/doc/client_api/group.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/client_api/miscellaneous.rst` & `pytango-9.4.2rc1/doc/client_api/miscellaneous.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/client_api/other.rst` & `pytango-9.4.2rc1/doc/client_api/other.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/conf.py` & `pytango-9.4.2rc1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/data_types.rst` & `pytango-9.4.2rc1/doc/data_types.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/exception.rst` & `pytango-9.4.2rc1/doc/exception.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/faq.rst` & `pytango-9.4.2rc1/doc/faq.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/green_modes/client_asyncio_mode.rst` & `pytango-9.4.2rc1/doc/green_modes/client_asyncio_mode.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/green_modes/client_futures_mode.rst` & `pytango-9.4.2rc1/doc/green_modes/client_futures_mode.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/green_modes/client_gevent_mode.rst` & `pytango-9.4.2rc1/doc/green_modes/client_gevent_mode.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/green_modes/green.rst` & `pytango-9.4.2rc1/doc/green_modes/green.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/green_modes/green_modes_client.rst` & `pytango-9.4.2rc1/doc/green_modes/green_modes_client.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/green_modes/green_modes_server.rst` & `pytango-9.4.2rc1/doc/green_modes/green_modes_server.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/how-to-contribute.rst` & `pytango-9.4.2rc1/doc/how-to-contribute.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/howto.rst` & `pytango-9.4.2rc1/doc/howto.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/itango.rst` & `pytango-9.4.2rc1/doc/itango.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/logo-medium.bmp` & `pytango-9.4.2rc1/doc/logo-medium.bmp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/migration/to-9.4/attr-decorators.rst` & `pytango-9.4.2rc1/doc/migration/to-9.4/attr-decorators.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/migration/to-9.4/deps-install.rst` & `pytango-9.4.2rc1/doc/migration/to-9.4/deps-install.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/migration/to-9.4/empty-attrs.rst` & `pytango-9.4.2rc1/doc/migration/to-9.4/empty-attrs.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/migration/to-9.4/extract-as.rst` & `pytango-9.4.2rc1/doc/migration/to-9.4/extract-as.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/migration/to-9.4/hl-dev-enum.rst` & `pytango-9.4.2rc1/doc/migration/to-9.4/hl-dev-enum.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/migration/to-9.4/hl-dynamic.rst` & `pytango-9.4.2rc1/doc/migration/to-9.4/hl-dynamic.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/migration/to-9.4/logging-percent-sym.rst` & `pytango-9.4.2rc1/doc/migration/to-9.4/logging-percent-sym.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/migration/to-9.4/non-bound-user-funcs.rst` & `pytango-9.4.2rc1/doc/migration/to-9.4/non-bound-user-funcs.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/migration/to-9.4/optional-proxy-attrs.rst` & `pytango-9.4.2rc1/doc/migration/to-9.4/optional-proxy-attrs.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/mock_tango_extension.py` & `pytango-9.4.2rc1/doc/mock_tango_extension.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/news.rst` & `pytango-9.4.2rc1/doc/news.rst`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     History of changes <revision>
 
 
 ****************************
 What's new in PyTango 9.4.2?
 ****************************
 
-Date: 2023-07-27
+Date: 2023-07-??
 
 Type: minor release
 
 Changed
 =======
 
 - New python and NumPy :ref:`version policy <pytango-version-policy>` is implemented.
```

### Comparing `pytango-9.4.2/doc/quicktour.rst` & `pytango-9.4.2rc1/doc/quicktour.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/revision.rst` & `pytango-9.4.2rc1/doc/revision.rst`

 * *Files 0% similar despite different names*

```diff
@@ -117,26 +117,26 @@
 +----------+----------------------------------------------------------------------------------+-----------------------------------------------------+-----------------------------------+
 | 28/09/22 | `9.3.6 <http://pytango.readthedocs.io/en/v9.3.6>`_                               | 9.3.6 Release                                       | Y\. Matveev                       |
 +----------+----------------------------------------------------------------------------------+-----------------------------------------------------+-----------------------------------+
 | 15/02/23 | `9.4.0 <http://pytango.readthedocs.io/en/v9.4.0>`_                               | 9.4.0 Release                                       | A\. Joubert                       |
 +----------+----------------------------------------------------------------------------------+-----------------------------------------------------+-----------------------------------+
 | 15/03/23 | `9.4.1 <http://pytango.readthedocs.io/en/v9.4.1>`_                               | 9.4.1 Release                                       | A\. Joubert                       |
 +----------+----------------------------------------------------------------------------------+-----------------------------------------------------+-----------------------------------+
-| 27/07/23 | `9.4.2 <http://pytango.readthedocs.io/en/v9.4.2>`_                               | 9.4.2 Release                                       | Y\. Matveev                       |
+| ??/07/23 | `9.4.2 <http://pytango.readthedocs.io/en/v9.4.2>`_                               | 9.4.2 Release                                       | Y\. Matveev                       |
 +----------+----------------------------------------------------------------------------------+-----------------------------------------------------+-----------------------------------+
 
 .. _pytango-version-history:
 
 Version history
 ---------------
 
 +----------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
 | Version  | Changes                                                                                                                                                                             |
 +==========+=====================================================================================================================================================================================+
-| 9.4.2    | 9.4.2 release.                                                                                                                                                                      |
+| 9.4.2rc1 | Release candidate 1 for 9.4.2.                                                                                                                                                      |
 |          |                                                                                                                                                                                     |
 |          | Features:                                                                                                                                                                           |
 |          |     - `!578: Add server init hook to high-level and low-level devices <https://gitlab.com/tango-controls/pytango/-/merge_requests/578>`_                                            |
 |          |     - `!562: Check code coverage <https://gitlab.com/tango-controls/pytango/-/merge_requests/562>`_                                                                                 |
 |          |     - `!577: Implement new python and NumPy version policy <https://gitlab.com/tango-controls/pytango/-/merge_requests/577>`_                                                       |
 |          |                                                                                                                                                                                     |
 |          | Bug fixes and changes:                                                                                                                                                              |
@@ -148,30 +148,27 @@
 |          |     - `!570: Fix linter problem in winsetup.py <https://gitlab.com/tango-controls/pytango/-/merge_requests/570>`_                                                                   |
 |          |     - `!579: Extend "empty string workaround" to sequences for DeviceTestContext properties <https://gitlab.com/tango-controls/pytango/-/merge_requests/579>`_                      |
 |          |                                                                                                                                                                                     |
 |          | Doc fixes:                                                                                                                                                                          |
 |          |     - `!571: Update new build system doc <https://gitlab.com/tango-controls/pytango/-/merge_requests/571>`_                                                                         |
 |          |     - `!572: Improve docs for push_data_ready_event and EnsureOmniThread <https://gitlab.com/tango-controls/pytango/-/merge_requests/572>`_                                         |
 |          |     - `!587: Update docs and bump version for 9.4.2rc1 <https://gitlab.com/tango-controls/pytango/-/merge_requests/587>`_                                                           |
-|          |     - `!595: Fixed history of changes <https://gitlab.com/tango-controls/pytango/-/merge_requests/595>`_                                                                            |
 |          |                                                                                                                                                                                     |
 |          |                                                                                                                                                                                     |
 |          | DevOps changes:                                                                                                                                                                     |
 |          |     - `!563: Skip log location tests in AppVeyor CI <https://gitlab.com/tango-controls/pytango/-/merge_requests/563>`_                                                              |
 |          |     - `!566: Add AppVeyor Windows builds for Python 3.9 to 3.11, Boost 1.82.0 <https://gitlab.com/tango-controls/pytango/-/merge_requests/566>`_                                    |
 |          |     - `!575: Add job to test main cpptango branch <https://gitlab.com/tango-controls/pytango/-/merge_requests/575>`_                                                                |
 |          |     - `!574: Added test for checking default and non-default units <https://gitlab.com/tango-controls/pytango/-/merge_requests/574>`_                                               |
 |          |     - `!576: Add macOS wheels + gitlab-ci cleaning <https://gitlab.com/tango-controls/pytango/-/merge_requests/576>`_                                                               |
 |          |     - `!585: Move to cppTango 9.4.2, drop Python<3.9 on Win, update wheel deps <https://gitlab.com/tango-controls/pytango/-/merge_requests/585>`_                                   |
-|          |     - `!588: Skip failing test in Winodws <https://gitlab.com/tango-controls/pytango/-/merge_requests/588>`_                                                                        |
-|          |     - `!593: Test_server_init_hook_subscribe_event_multiple_devices skiped <https://gitlab.com/tango-controls/pytango/-/merge_requests/593>`_                                       |
 |          |                                                                                                                                                                                     |
 |          | More details in the `full changelog 9.4.1...9.4.2 <https://gitlab.com/tango-controls/pytango/-/compare/v9.4.1...v9.4.2>`_                                                           |
 |          |                                                                                                                                                                                     |
-+----------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
++==========+=====================================================================================================================================================================================+
 | 9.4.1    | 9.4.1 release.                                                                                                                                                                      |
 |          |                                                                                                                                                                                     |
 |          | Bug fixes and changes:                                                                                                                                                              |
 |          |     - `!547: Fix attributes with device inheritance and repeated method wrapping regression in 9.4.0 <https://gitlab.com/tango-controls/pytango/-/merge_requests/547>`_             |
 |          |     - `!548: Fix decorated attribute methods regression in 9.4.0 <https://gitlab.com/tango-controls/pytango/-/merge_requests/548>`_                                                 |
 |          |                                                                                                                                                                                     |
 |          | Doc fixes:                                                                                                                                                                          |
```

### Comparing `pytango-9.4.2/doc/server_api/server.rst` & `pytango-9.4.2rc1/doc/server_api/server.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/start.rst` & `pytango-9.4.2rc1/doc/start.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/tep/DataBase.xmi` & `pytango-9.4.2rc1/doc/tep/DataBase.xmi`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/tep/database.py` & `pytango-9.4.2rc1/doc/tep/database.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/tep/tep-0001.rst` & `pytango-9.4.2rc1/doc/tep/tep-0001.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/tep/tep-0002.rst` & `pytango-9.4.2rc1/doc/tep/tep-0002.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/testing/coverage.rst` & `pytango-9.4.2rc1/doc/testing/coverage.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/testing/mocks.rst` & `pytango-9.4.2rc1/doc/testing/mocks.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/testing/test_context.rst` & `pytango-9.4.2rc1/doc/testing/test_context.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/testing/testing_approaches.rst` & `pytango-9.4.2rc1/doc/testing/testing_approaches.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/utilities.rst` & `pytango-9.4.2rc1/doc/utilities.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/version-policy.rst` & `pytango-9.4.2rc1/doc/version-policy.rst`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/doc/windows_notes.txt` & `pytango-9.4.2rc1/doc/windows_notes.txt`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/Clock/ClockDS.py` & `pytango-9.4.2rc1/examples/Clock/ClockDS.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/Clock/client.py` & `pytango-9.4.2rc1/examples/Clock/client.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/TuringMachine/TuringMachine.py` & `pytango-9.4.2rc1/examples/TuringMachine/TuringMachine.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/asyncio_green_mode/asyncio_device_example.py` & `pytango-9.4.2rc1/examples/asyncio_green_mode/asyncio_device_example.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/asyncio_green_mode/tcp_server_example.py` & `pytango-9.4.2rc1/examples/asyncio_green_mode/tcp_server_example.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/dynamic/dynamic_client.py` & `pytango-9.4.2rc1/examples/dynamic/dynamic_client.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/dynamic/dynamic_server.py` & `pytango-9.4.2rc1/examples/dynamic/dynamic_server.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/fwdAttr/FwdServer.py` & `pytango-9.4.2rc1/examples/fwdAttr/FwdServer.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/interfacechangeEvents/ClassFactory.cpp` & `pytango-9.4.2rc1/examples/interfacechangeEvents/ClassFactory.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/interfacechangeEvents/IfchangeClient.py` & `pytango-9.4.2rc1/examples/interfacechangeEvents/IfchangeClient.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/interfacechangeEvents/IfchangeServer.cpp` & `pytango-9.4.2rc1/examples/interfacechangeEvents/IfchangeServer.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/interfacechangeEvents/IfchangeServer.h` & `pytango-9.4.2rc1/examples/interfacechangeEvents/IfchangeServer.h`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/interfacechangeEvents/IfchangeServer.py` & `pytango-9.4.2rc1/examples/interfacechangeEvents/IfchangeServer.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/interfacechangeEvents/IfchangeServer.xmi` & `pytango-9.4.2rc1/examples/interfacechangeEvents/IfchangeServer.xmi`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/interfacechangeEvents/IfchangeServerClass.cpp` & `pytango-9.4.2rc1/examples/interfacechangeEvents/IfchangeServerClass.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/interfacechangeEvents/IfchangeServerClass.h` & `pytango-9.4.2rc1/examples/interfacechangeEvents/IfchangeServerClass.h`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/interfacechangeEvents/IfchangeServerDynAttrUtils.cpp` & `pytango-9.4.2rc1/examples/interfacechangeEvents/IfchangeServerDynAttrUtils.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/interfacechangeEvents/IfchangeServerStateMachine.cpp` & `pytango-9.4.2rc1/examples/interfacechangeEvents/IfchangeServerStateMachine.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/interfacechangeEvents/Makefile` & `pytango-9.4.2rc1/examples/interfacechangeEvents/Makefile`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/interfacechangeEvents/Makefile.bck` & `pytango-9.4.2rc1/examples/interfacechangeEvents/Makefile.bck`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/interfacechangeEvents/main.cpp` & `pytango-9.4.2rc1/examples/interfacechangeEvents/main.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/mandatory/MandatoryPropertyServer.py` & `pytango-9.4.2rc1/examples/mandatory/MandatoryPropertyServer.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/many/many_server.py` & `pytango-9.4.2rc1/examples/many/many_server.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/multi/multi_client.py` & `pytango-9.4.2rc1/examples/multi/multi_client.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/multi/multi_server.py` & `pytango-9.4.2rc1/examples/multi/multi_server.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/multidevicetestcontext/conftest.py` & `pytango-9.4.2rc1/examples/multidevicetestcontext/conftest.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/multidevicetestcontext/test_integration.py` & `pytango-9.4.2rc1/examples/multidevicetestcontext/test_integration.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/pipeEvents/ClassFactory.cpp` & `pytango-9.4.2rc1/examples/pipeEvents/ClassFactory.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/pipeEvents/Makefile` & `pytango-9.4.2rc1/examples/pipeEvents/Makefile`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/pipeEvents/PipeEventClient.py` & `pytango-9.4.2rc1/examples/pipeEvents/PipeEventClient.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/pipeEvents/PipeServer.cpp` & `pytango-9.4.2rc1/examples/pipeEvents/PipeServer.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/pipeEvents/PipeServer.h` & `pytango-9.4.2rc1/examples/pipeEvents/PipeServer.h`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/pipeEvents/PipeServer.py` & `pytango-9.4.2rc1/examples/pipeEvents/PipeServer.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/pipeEvents/PipeServer.xmi` & `pytango-9.4.2rc1/examples/pipeEvents/PipeServer.xmi`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/pipeEvents/PipeServerClass.cpp` & `pytango-9.4.2rc1/examples/pipeEvents/PipeServerClass.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/pipeEvents/PipeServerClass.h` & `pytango-9.4.2rc1/examples/pipeEvents/PipeServerClass.h`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/pipeEvents/PipeServerStateMachine.cpp` & `pytango-9.4.2rc1/examples/pipeEvents/PipeServerStateMachine.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/pipeEvents/main.cpp` & `pytango-9.4.2rc1/examples/pipeEvents/main.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/pipes/ClassFactory.cpp` & `pytango-9.4.2rc1/examples/pipes/ClassFactory.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/pipes/Makefile` & `pytango-9.4.2rc1/examples/pipes/Makefile`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/pipes/PipeClient.py` & `pytango-9.4.2rc1/examples/pipes/PipeClient.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/pipes/PipeServer.cpp` & `pytango-9.4.2rc1/examples/pipes/PipeServer.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/pipes/PipeServer.h` & `pytango-9.4.2rc1/examples/pipes/PipeServer.h`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/pipes/PipeServer.py` & `pytango-9.4.2rc1/examples/pipes/PipeServer.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/pipes/PipeServer.xmi` & `pytango-9.4.2rc1/examples/pipes/PipeServer.xmi`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/pipes/PipeServerClass.cpp` & `pytango-9.4.2rc1/examples/pipes/PipeServerClass.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/pipes/PipeServerClass.h` & `pytango-9.4.2rc1/examples/pipes/PipeServerClass.h`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/pipes/PipeServerStateMachine.cpp` & `pytango-9.4.2rc1/examples/pipes/PipeServerStateMachine.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/pipes/main.cpp` & `pytango-9.4.2rc1/examples/pipes/main.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/simple/simple_client.py` & `pytango-9.4.2rc1/examples/simple/simple_client.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/simple/simple_server.py` & `pytango-9.4.2rc1/examples/simple/simple_server.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/training/README.md` & `pytango-9.4.2rc1/examples/training/README.md`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/training/client/command01.py` & `pytango-9.4.2rc1/examples/training/client/command01.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/training/client/command02.py` & `pytango-9.4.2rc1/examples/training/client/command02.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/training/client/reading01.py` & `pytango-9.4.2rc1/examples/training/client/reading01.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/training/client/reading02.py` & `pytango-9.4.2rc1/examples/training/client/reading02.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/training/client/reading03.py` & `pytango-9.4.2rc1/examples/training/client/reading03.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/training/client/writing01.py` & `pytango-9.4.2rc1/examples/training/client/writing01.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/training/client/writing02.py` & `pytango-9.4.2rc1/examples/training/client/writing02.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/training/docker-compose.yml` & `pytango-9.4.2rc1/examples/training/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/training/server/libps.py` & `pytango-9.4.2rc1/examples/training/server/libps.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/training/server/low-level-api.py` & `pytango-9.4.2rc1/examples/training/server/low-level-api.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/training/server/ps-simulator.py` & `pytango-9.4.2rc1/examples/training/server/ps-simulator.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/training/server/ps0b-push-event.py` & `pytango-9.4.2rc1/examples/training/server/ps0b-push-event.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/training/server/ps0b.py` & `pytango-9.4.2rc1/examples/training/server/ps0b.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/training/server/ps0c.py` & `pytango-9.4.2rc1/examples/training/server/ps0c.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/training/server/ps1-gevent.py` & `pytango-9.4.2rc1/examples/training/server/ps1-gevent.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/training/server/ps1-use-lib-logging.py` & `pytango-9.4.2rc1/examples/training/server/ps1-use-lib-logging.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/training/server/ps1-use-lib.py` & `pytango-9.4.2rc1/examples/training/server/ps1-use-lib.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/training/server/ps1.py` & `pytango-9.4.2rc1/examples/training/server/ps1.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/training/server/ps2-gevent-check.py` & `pytango-9.4.2rc1/examples/training/server/ps2-gevent-check.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/training/server/ps2-gevent.py` & `pytango-9.4.2rc1/examples/training/server/ps2-gevent.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/training/server/test_ps0b.py` & `pytango-9.4.2rc1/examples/training/server/test_ps0b.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/training/webinars/crash_example.py` & `pytango-9.4.2rc1/examples/training/webinars/crash_example.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/examples/training/webinars/test_webinar.py` & `pytango-9.4.2rc1/examples/training/webinars/test_webinar.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/api_util.cpp` & `pytango-9.4.2rc1/ext/api_util.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/archive_event_info.cpp` & `pytango-9.4.2rc1/ext/archive_event_info.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/attr_conf_event_data.cpp` & `pytango-9.4.2rc1/ext/attr_conf_event_data.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/attribute_alarm_info.cpp` & `pytango-9.4.2rc1/ext/attribute_alarm_info.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/attribute_dimension.cpp` & `pytango-9.4.2rc1/ext/attribute_dimension.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/attribute_event_info.cpp` & `pytango-9.4.2rc1/ext/attribute_event_info.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/attribute_info.cpp` & `pytango-9.4.2rc1/ext/attribute_info.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/attribute_info_ex.cpp` & `pytango-9.4.2rc1/ext/attribute_info_ex.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/attribute_proxy.cpp` & `pytango-9.4.2rc1/ext/attribute_proxy.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/base_types.cpp` & `pytango-9.4.2rc1/ext/base_types.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/base_types_numpy.hpp` & `pytango-9.4.2rc1/ext/base_types_numpy.hpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/callback.cpp` & `pytango-9.4.2rc1/ext/callback.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/callback.h` & `pytango-9.4.2rc1/ext/callback.h`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/change_event_info.cpp` & `pytango-9.4.2rc1/ext/change_event_info.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/command_info.cpp` & `pytango-9.4.2rc1/ext/command_info.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/connection.cpp` & `pytango-9.4.2rc1/ext/connection.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/constants.cpp` & `pytango-9.4.2rc1/ext/constants.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/data_ready_event_data.cpp` & `pytango-9.4.2rc1/ext/data_ready_event_data.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/database.cpp` & `pytango-9.4.2rc1/ext/database.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/db.cpp` & `pytango-9.4.2rc1/ext/db.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/defs.h` & `pytango-9.4.2rc1/ext/defs.h`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/dev_command_info.cpp` & `pytango-9.4.2rc1/ext/dev_command_info.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/dev_error.cpp` & `pytango-9.4.2rc1/ext/dev_error.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/device_attribute.cpp` & `pytango-9.4.2rc1/ext/device_attribute.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/device_attribute.h` & `pytango-9.4.2rc1/ext/device_attribute.h`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/device_attribute_config.cpp` & `pytango-9.4.2rc1/ext/device_attribute_config.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/device_attribute_history.cpp` & `pytango-9.4.2rc1/ext/device_attribute_history.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/device_attribute_numpy.hpp` & `pytango-9.4.2rc1/ext/device_attribute_numpy.hpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/device_data.cpp` & `pytango-9.4.2rc1/ext/device_data.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/device_data_history.cpp` & `pytango-9.4.2rc1/ext/device_data_history.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/device_info.cpp` & `pytango-9.4.2rc1/ext/device_info.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/device_pipe.cpp` & `pytango-9.4.2rc1/ext/device_pipe.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/device_pipe.h` & `pytango-9.4.2rc1/ext/device_pipe.h`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/device_proxy.cpp` & `pytango-9.4.2rc1/ext/device_proxy.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/devintr_change_event_data.cpp` & `pytango-9.4.2rc1/ext/devintr_change_event_data.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/enums.cpp` & `pytango-9.4.2rc1/ext/enums.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/event_data.cpp` & `pytango-9.4.2rc1/ext/event_data.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/exception.cpp` & `pytango-9.4.2rc1/ext/exception.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/exception.h` & `pytango-9.4.2rc1/ext/exception.h`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/fast_from_py.h` & `pytango-9.4.2rc1/ext/fast_from_py.h`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/fast_from_py_numpy.hpp` & `pytango-9.4.2rc1/ext/fast_from_py_numpy.hpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/from_py.cpp` & `pytango-9.4.2rc1/ext/from_py.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/from_py.h` & `pytango-9.4.2rc1/ext/from_py.h`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/group.cpp` & `pytango-9.4.2rc1/ext/group.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/group_reply.cpp` & `pytango-9.4.2rc1/ext/group_reply.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/group_reply_list.cpp` & `pytango-9.4.2rc1/ext/group_reply_list.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/locker_info.cpp` & `pytango-9.4.2rc1/ext/locker_info.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/locking_thread.cpp` & `pytango-9.4.2rc1/ext/locking_thread.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/periodic_event_info.cpp` & `pytango-9.4.2rc1/ext/periodic_event_info.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/pipe_event_data.cpp` & `pytango-9.4.2rc1/ext/pipe_event_data.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/pipe_info.cpp` & `pytango-9.4.2rc1/ext/pipe_info.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/poll_device.cpp` & `pytango-9.4.2rc1/ext/poll_device.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/precompiled_header.cpp` & `pytango-9.4.2rc1/ext/precompiled_header.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/precompiled_header.hpp` & `pytango-9.4.2rc1/ext/precompiled_header.hpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/pytango.cpp` & `pytango-9.4.2rc1/ext/pytango.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/pytgutils.cpp` & `pytango-9.4.2rc1/ext/pytgutils.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/pytgutils.h` & `pytango-9.4.2rc1/ext/pytgutils.h`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/pyutils.cpp` & `pytango-9.4.2rc1/ext/pyutils.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/pyutils.h` & `pytango-9.4.2rc1/ext/pyutils.h`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/server/attr.cpp` & `pytango-9.4.2rc1/ext/server/attr.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/server/attr.h` & `pytango-9.4.2rc1/ext/server/attr.h`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/server/attribute.cpp` & `pytango-9.4.2rc1/ext/server/attribute.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/server/attribute.h` & `pytango-9.4.2rc1/ext/server/attribute.h`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/server/auto_monitor.cpp` & `pytango-9.4.2rc1/ext/server/auto_monitor.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/server/command.cpp` & `pytango-9.4.2rc1/ext/server/command.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/server/command.h` & `pytango-9.4.2rc1/ext/server/command.h`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/server/device_class.cpp` & `pytango-9.4.2rc1/ext/server/device_class.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/server/device_class.h` & `pytango-9.4.2rc1/ext/server/device_class.h`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/server/device_impl.cpp` & `pytango-9.4.2rc1/ext/server/device_impl.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/server/device_impl.h` & `pytango-9.4.2rc1/ext/server/device_impl.h`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/server/dserver.cpp` & `pytango-9.4.2rc1/ext/server/dserver.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/server/encoded_attribute.cpp` & `pytango-9.4.2rc1/ext/server/encoded_attribute.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/server/fwdAttr.cpp` & `pytango-9.4.2rc1/ext/server/fwdAttr.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/server/log4tango.cpp` & `pytango-9.4.2rc1/ext/server/log4tango.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/server/multi_attribute.cpp` & `pytango-9.4.2rc1/ext/server/multi_attribute.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/server/multi_class_attribute.cpp` & `pytango-9.4.2rc1/ext/server/multi_class_attribute.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/server/pipe.cpp` & `pytango-9.4.2rc1/ext/server/pipe.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/server/pipe.h` & `pytango-9.4.2rc1/ext/server/pipe.h`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/server/subdev.cpp` & `pytango-9.4.2rc1/ext/server/subdev.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/server/tango_util.cpp` & `pytango-9.4.2rc1/ext/server/tango_util.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/server/user_default_attr_prop.cpp` & `pytango-9.4.2rc1/ext/server/user_default_attr_prop.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/server/user_default_pipe_prop.cpp` & `pytango-9.4.2rc1/ext/server/user_default_pipe_prop.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/server/wattribute.cpp` & `pytango-9.4.2rc1/ext/server/wattribute.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/server/wattribute_numpy.hpp` & `pytango-9.4.2rc1/ext/server/wattribute_numpy.hpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/tango_numpy.h` & `pytango-9.4.2rc1/ext/tango_numpy.h`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/tgutils.h` & `pytango-9.4.2rc1/ext/tgutils.h`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/time_val.cpp` & `pytango-9.4.2rc1/ext/time_val.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/to_py.cpp` & `pytango-9.4.2rc1/ext/to_py.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/to_py.h` & `pytango-9.4.2rc1/ext/to_py.h`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/to_py_numpy.hpp` & `pytango-9.4.2rc1/ext/to_py_numpy.hpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/ext/version.cpp` & `pytango-9.4.2rc1/ext/version.cpp`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/pyproject.toml` & `pytango-9.4.2rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/pytango.egg-info/PKG-INFO` & `pytango-9.4.2rc1/pytango.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pytango
-Version: 9.4.2
+Version: 9.4.2rc1
 Summary: A python binding for the Tango control system
 Home-page: http://gitlab.com/tango-controls/pytango
+Download-URL: http://pypi.python.org/pypi/pytango
 Author: Tiago Coutinho
 Author-email: coutinho@esrf.fr
 License: LGPL
-Download-URL: http://pypi.python.org/pypi/pytango
 Keywords: Tango,CORBA,binding
 Platform: Linux
 Platform: Windows XP/Vista/7/8/10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
@@ -185,8 +185,7 @@
 .. _IPython: http://ipython.org
 
 .. _documentation: http://pytango.readthedocs.io/en/latest
 .. _Tango forums: http://tango-controls.org/community/forum
 .. _PR and bug reports: PyTango_
 .. _sources: PyTango_
 .. _How to Contribute: http://pytango.readthedocs.io/en/latest/how-to-contribute.html#how-to-contribute
-
```

### Comparing `pytango-9.4.2/pytango.egg-info/SOURCES.txt` & `pytango-9.4.2rc1/pytango.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -4,81 +4,81 @@
 Makefile
 PyTango.py
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
 winsetup.py
-/builds/tango-controls/pytango/ext/api_util.cpp
-/builds/tango-controls/pytango/ext/archive_event_info.cpp
-/builds/tango-controls/pytango/ext/attr_conf_event_data.cpp
-/builds/tango-controls/pytango/ext/attribute_alarm_info.cpp
-/builds/tango-controls/pytango/ext/attribute_dimension.cpp
-/builds/tango-controls/pytango/ext/attribute_event_info.cpp
-/builds/tango-controls/pytango/ext/attribute_info.cpp
-/builds/tango-controls/pytango/ext/attribute_info_ex.cpp
-/builds/tango-controls/pytango/ext/attribute_proxy.cpp
-/builds/tango-controls/pytango/ext/base_types.cpp
-/builds/tango-controls/pytango/ext/callback.cpp
-/builds/tango-controls/pytango/ext/change_event_info.cpp
-/builds/tango-controls/pytango/ext/command_info.cpp
-/builds/tango-controls/pytango/ext/connection.cpp
-/builds/tango-controls/pytango/ext/constants.cpp
-/builds/tango-controls/pytango/ext/data_ready_event_data.cpp
-/builds/tango-controls/pytango/ext/database.cpp
-/builds/tango-controls/pytango/ext/db.cpp
-/builds/tango-controls/pytango/ext/dev_command_info.cpp
-/builds/tango-controls/pytango/ext/dev_error.cpp
-/builds/tango-controls/pytango/ext/device_attribute.cpp
-/builds/tango-controls/pytango/ext/device_attribute_config.cpp
-/builds/tango-controls/pytango/ext/device_attribute_history.cpp
-/builds/tango-controls/pytango/ext/device_data.cpp
-/builds/tango-controls/pytango/ext/device_data_history.cpp
-/builds/tango-controls/pytango/ext/device_info.cpp
-/builds/tango-controls/pytango/ext/device_pipe.cpp
-/builds/tango-controls/pytango/ext/device_proxy.cpp
-/builds/tango-controls/pytango/ext/devintr_change_event_data.cpp
-/builds/tango-controls/pytango/ext/enums.cpp
-/builds/tango-controls/pytango/ext/event_data.cpp
-/builds/tango-controls/pytango/ext/exception.cpp
-/builds/tango-controls/pytango/ext/from_py.cpp
-/builds/tango-controls/pytango/ext/group.cpp
-/builds/tango-controls/pytango/ext/group_reply.cpp
-/builds/tango-controls/pytango/ext/group_reply_list.cpp
-/builds/tango-controls/pytango/ext/locker_info.cpp
-/builds/tango-controls/pytango/ext/locking_thread.cpp
-/builds/tango-controls/pytango/ext/periodic_event_info.cpp
-/builds/tango-controls/pytango/ext/pipe_event_data.cpp
-/builds/tango-controls/pytango/ext/pipe_info.cpp
-/builds/tango-controls/pytango/ext/poll_device.cpp
-/builds/tango-controls/pytango/ext/precompiled_header.cpp
-/builds/tango-controls/pytango/ext/pytango.cpp
-/builds/tango-controls/pytango/ext/pytgutils.cpp
-/builds/tango-controls/pytango/ext/pyutils.cpp
-/builds/tango-controls/pytango/ext/time_val.cpp
-/builds/tango-controls/pytango/ext/to_py.cpp
-/builds/tango-controls/pytango/ext/version.cpp
-/builds/tango-controls/pytango/ext/server/attr.cpp
-/builds/tango-controls/pytango/ext/server/attribute.cpp
-/builds/tango-controls/pytango/ext/server/auto_monitor.cpp
-/builds/tango-controls/pytango/ext/server/command.cpp
-/builds/tango-controls/pytango/ext/server/device_class.cpp
-/builds/tango-controls/pytango/ext/server/device_impl.cpp
-/builds/tango-controls/pytango/ext/server/dserver.cpp
-/builds/tango-controls/pytango/ext/server/encoded_attribute.cpp
-/builds/tango-controls/pytango/ext/server/fwdAttr.cpp
-/builds/tango-controls/pytango/ext/server/log4tango.cpp
-/builds/tango-controls/pytango/ext/server/multi_attribute.cpp
-/builds/tango-controls/pytango/ext/server/multi_class_attribute.cpp
-/builds/tango-controls/pytango/ext/server/pipe.cpp
-/builds/tango-controls/pytango/ext/server/subdev.cpp
-/builds/tango-controls/pytango/ext/server/tango_util.cpp
-/builds/tango-controls/pytango/ext/server/user_default_attr_prop.cpp
-/builds/tango-controls/pytango/ext/server/user_default_pipe_prop.cpp
-/builds/tango-controls/pytango/ext/server/wattribute.cpp
+/home/matveyev/pytango/ext/api_util.cpp
+/home/matveyev/pytango/ext/archive_event_info.cpp
+/home/matveyev/pytango/ext/attr_conf_event_data.cpp
+/home/matveyev/pytango/ext/attribute_alarm_info.cpp
+/home/matveyev/pytango/ext/attribute_dimension.cpp
+/home/matveyev/pytango/ext/attribute_event_info.cpp
+/home/matveyev/pytango/ext/attribute_info.cpp
+/home/matveyev/pytango/ext/attribute_info_ex.cpp
+/home/matveyev/pytango/ext/attribute_proxy.cpp
+/home/matveyev/pytango/ext/base_types.cpp
+/home/matveyev/pytango/ext/callback.cpp
+/home/matveyev/pytango/ext/change_event_info.cpp
+/home/matveyev/pytango/ext/command_info.cpp
+/home/matveyev/pytango/ext/connection.cpp
+/home/matveyev/pytango/ext/constants.cpp
+/home/matveyev/pytango/ext/data_ready_event_data.cpp
+/home/matveyev/pytango/ext/database.cpp
+/home/matveyev/pytango/ext/db.cpp
+/home/matveyev/pytango/ext/dev_command_info.cpp
+/home/matveyev/pytango/ext/dev_error.cpp
+/home/matveyev/pytango/ext/device_attribute.cpp
+/home/matveyev/pytango/ext/device_attribute_config.cpp
+/home/matveyev/pytango/ext/device_attribute_history.cpp
+/home/matveyev/pytango/ext/device_data.cpp
+/home/matveyev/pytango/ext/device_data_history.cpp
+/home/matveyev/pytango/ext/device_info.cpp
+/home/matveyev/pytango/ext/device_pipe.cpp
+/home/matveyev/pytango/ext/device_proxy.cpp
+/home/matveyev/pytango/ext/devintr_change_event_data.cpp
+/home/matveyev/pytango/ext/enums.cpp
+/home/matveyev/pytango/ext/event_data.cpp
+/home/matveyev/pytango/ext/exception.cpp
+/home/matveyev/pytango/ext/from_py.cpp
+/home/matveyev/pytango/ext/group.cpp
+/home/matveyev/pytango/ext/group_reply.cpp
+/home/matveyev/pytango/ext/group_reply_list.cpp
+/home/matveyev/pytango/ext/locker_info.cpp
+/home/matveyev/pytango/ext/locking_thread.cpp
+/home/matveyev/pytango/ext/periodic_event_info.cpp
+/home/matveyev/pytango/ext/pipe_event_data.cpp
+/home/matveyev/pytango/ext/pipe_info.cpp
+/home/matveyev/pytango/ext/poll_device.cpp
+/home/matveyev/pytango/ext/precompiled_header.cpp
+/home/matveyev/pytango/ext/pytango.cpp
+/home/matveyev/pytango/ext/pytgutils.cpp
+/home/matveyev/pytango/ext/pyutils.cpp
+/home/matveyev/pytango/ext/time_val.cpp
+/home/matveyev/pytango/ext/to_py.cpp
+/home/matveyev/pytango/ext/version.cpp
+/home/matveyev/pytango/ext/server/attr.cpp
+/home/matveyev/pytango/ext/server/attribute.cpp
+/home/matveyev/pytango/ext/server/auto_monitor.cpp
+/home/matveyev/pytango/ext/server/command.cpp
+/home/matveyev/pytango/ext/server/device_class.cpp
+/home/matveyev/pytango/ext/server/device_impl.cpp
+/home/matveyev/pytango/ext/server/dserver.cpp
+/home/matveyev/pytango/ext/server/encoded_attribute.cpp
+/home/matveyev/pytango/ext/server/fwdAttr.cpp
+/home/matveyev/pytango/ext/server/log4tango.cpp
+/home/matveyev/pytango/ext/server/multi_attribute.cpp
+/home/matveyev/pytango/ext/server/multi_class_attribute.cpp
+/home/matveyev/pytango/ext/server/pipe.cpp
+/home/matveyev/pytango/ext/server/subdev.cpp
+/home/matveyev/pytango/ext/server/tango_util.cpp
+/home/matveyev/pytango/ext/server/user_default_attr_prop.cpp
+/home/matveyev/pytango/ext/server/user_default_pipe_prop.cpp
+/home/matveyev/pytango/ext/server/wattribute.cpp
 cmake/project_version.cc.in
 cmake/project_version.cmake
 cmake/project_version.h.in
 doc/api.rst
 doc/conf.py
 doc/contents.rst
 doc/data_types.rst
@@ -296,17 +296,19 @@
 ext/database.cpp
 ext/db.cpp
 ext/defs.h
 ext/dev_command_info.cpp
 ext/dev_error.cpp
 ext/device_attribute.cpp
 ext/device_attribute.h
+ext/device_attribute.h.gch
 ext/device_attribute_config.cpp
 ext/device_attribute_history.cpp
 ext/device_attribute_numpy.hpp
+ext/device_attribute_numpy.hpp.gch
 ext/device_data.cpp
 ext/device_data_history.cpp
 ext/device_info.cpp
 ext/device_pipe.cpp
 ext/device_pipe.h
 ext/device_proxy.cpp
 ext/devintr_change_event_data.cpp
@@ -330,14 +332,15 @@
 ext/precompiled_header.cpp
 ext/precompiled_header.hpp
 ext/pytango.cpp
 ext/pytgutils.cpp
 ext/pytgutils.h
 ext/pyutils.cpp
 ext/pyutils.h
+ext/pyutils.h.gch
 ext/tango_numpy.h
 ext/tgutils.h
 ext/time_val.cpp
 ext/to_py.cpp
 ext/to_py.h
 ext/to_py_numpy.hpp
 ext/version.cpp
@@ -421,12 +424,13 @@
 tango/databaseds/create_db_tables.sql
 tango/databaseds/database.py
 tango/databaseds/db_errors.py
 tango/databaseds/mysql2sqlite.sh
 tango/databaseds/db_access/__init__.py
 tango/databaseds/db_access/sqlite3.py
 tests/conftest.py
+tests/report.xml
 tests/test_async.py
 tests/test_client.py
 tests/test_event.py
 tests/test_server.py
 tests/test_test_context.py
```

### Comparing `pytango-9.4.2/setup.py` & `pytango-9.4.2rc1/setup.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/tango/__init__.py` & `pytango-9.4.2rc1/tango/__init__.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/tango/api_util.py` & `pytango-9.4.2rc1/tango/api_util.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/tango/asyncio.py` & `pytango-9.4.2rc1/tango/asyncio.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/tango/asyncio_executor.py` & `pytango-9.4.2rc1/tango/asyncio_executor.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/tango/attr_data.py` & `pytango-9.4.2rc1/tango/attr_data.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/tango/attribute_proxy.py` & `pytango-9.4.2rc1/tango/attribute_proxy.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/tango/auto_monitor.py` & `pytango-9.4.2rc1/tango/auto_monitor.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/tango/base_types.py` & `pytango-9.4.2rc1/tango/base_types.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/tango/callback.py` & `pytango-9.4.2rc1/tango/callback.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/tango/client.py` & `pytango-9.4.2rc1/tango/client.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/tango/codec.py` & `pytango-9.4.2rc1/tango/codec.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/tango/connection.py` & `pytango-9.4.2rc1/tango/connection.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/tango/databaseds/DataBase.xmi` & `pytango-9.4.2rc1/tango/databaseds/DataBase.xmi`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/tango/databaseds/create_db.sql` & `pytango-9.4.2rc1/tango/databaseds/create_db.sql`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/tango/databaseds/create_db_tables.sql` & `pytango-9.4.2rc1/tango/databaseds/create_db_tables.sql`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/tango/databaseds/database.py` & `pytango-9.4.2rc1/tango/databaseds/database.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/tango/databaseds/db_access/sqlite3.py` & `pytango-9.4.2rc1/tango/databaseds/db_access/sqlite3.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/tango/databaseds/mysql2sqlite.sh` & `pytango-9.4.2rc1/tango/databaseds/mysql2sqlite.sh`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/tango/db.py` & `pytango-9.4.2rc1/tango/db.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/tango/device_attribute.py` & `pytango-9.4.2rc1/tango/device_attribute.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/tango/device_class.py` & `pytango-9.4.2rc1/tango/device_class.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/tango/device_data.py` & `pytango-9.4.2rc1/tango/device_data.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/tango/device_proxy.py` & `pytango-9.4.2rc1/tango/device_proxy.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/tango/device_server.py` & `pytango-9.4.2rc1/tango/device_server.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/tango/encoded_attribute.py` & `pytango-9.4.2rc1/tango/encoded_attribute.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/tango/exception.py` & `pytango-9.4.2rc1/tango/exception.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/tango/futures.py` & `pytango-9.4.2rc1/tango/futures.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/tango/futures_executor.py` & `pytango-9.4.2rc1/tango/futures_executor.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/tango/gevent.py` & `pytango-9.4.2rc1/tango/gevent.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/tango/gevent_executor.py` & `pytango-9.4.2rc1/tango/gevent_executor.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/tango/globals.py` & `pytango-9.4.2rc1/tango/globals.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/tango/green.py` & `pytango-9.4.2rc1/tango/green.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/tango/group.py` & `pytango-9.4.2rc1/tango/group.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/tango/group_reply.py` & `pytango-9.4.2rc1/tango/group_reply.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/tango/group_reply_list.py` & `pytango-9.4.2rc1/tango/group_reply_list.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/tango/log4tango.py` & `pytango-9.4.2rc1/tango/log4tango.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/tango/pipe.py` & `pytango-9.4.2rc1/tango/pipe.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/tango/pipe_data.py` & `pytango-9.4.2rc1/tango/pipe_data.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/tango/pytango_init.py` & `pytango-9.4.2rc1/tango/pytango_init.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/tango/pytango_pprint.py` & `pytango-9.4.2rc1/tango/pytango_pprint.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/tango/pyutil.py` & `pytango-9.4.2rc1/tango/pyutil.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/tango/release.py` & `pytango-9.4.2rc1/tango/release.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         - download_url: (str) package download url
         - platform: (seq<str>) list of available platforms
         - keywords: (seq<str>) list of keywords
         - license: (str) the license
     """
 
     name = "pytango"
-    version_info = (9, 4, 2)
+    version_info = (9, 4, 2, "rc", 1)
     version = ".".join(map(str, version_info[:3]))
     release = "".join(map(str, version_info[3:]))
     separator = "." if "dev" in release or "post" in release else ""
     version_long = version + separator + release
 
     version_description = "This version implements the C++ Tango 9.4 API."
     version_number = int(version.replace(".", ""))
```

### Comparing `pytango-9.4.2/tango/server.py` & `pytango-9.4.2rc1/tango/server.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/tango/tango_numpy.py` & `pytango-9.4.2rc1/tango/tango_numpy.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/tango/tango_object.py` & `pytango-9.4.2rc1/tango/tango_object.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/tango/test_context.py` & `pytango-9.4.2rc1/tango/test_context.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/tango/test_utils.py` & `pytango-9.4.2rc1/tango/test_utils.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/tango/time_val.py` & `pytango-9.4.2rc1/tango/time_val.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/tango/utils.py` & `pytango-9.4.2rc1/tango/utils.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/tests/conftest.py` & `pytango-9.4.2rc1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/tests/test_async.py` & `pytango-9.4.2rc1/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/tests/test_client.py` & `pytango-9.4.2rc1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/tests/test_event.py` & `pytango-9.4.2rc1/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/tests/test_server.py` & `pytango-9.4.2rc1/tests/test_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -3493,15 +3493,16 @@
     ):
         assert len(event_list) == 3
         assert "DeviceOne" in event_list
         assert "DeviceTwo" in event_list
 
 
 def test_server_init_hook_subscribe_event_multiple_devices():
-    pytest.xfail("This test fails in some systems, will be fixed soon")
+    if "win" in sys.platform:
+        pytest.xfail("This test fails in Windows, will be fixed soon")
 
     event_queue = multiprocessing.Queue()
 
     class DeviceOne(Device):
         @attribute(dtype=int)
         def some_attribute(self):
             return 42
```

### Comparing `pytango-9.4.2/tests/test_test_context.py` & `pytango-9.4.2rc1/tests/test_test_context.py`

 * *Files identical despite different names*

### Comparing `pytango-9.4.2/winsetup.py` & `pytango-9.4.2rc1/winsetup.py`

 * *Files identical despite different names*

