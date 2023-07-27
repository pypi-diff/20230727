# Comparing `tmp/django-storage-swift-1.2.9.tar.gz` & `tmp/django-storage-swift-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-storage-swift-1.2.9.tar", last modified: Tue Feb 16 10:20:45 2016, max compression
+gzip compressed data, was "django-storage-swift-1.3.0.tar", last modified: Thu Jul 27 19:15:39 2023, max compression
```

## Comparing `django-storage-swift-1.2.9.tar` & `django-storage-swift-1.3.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 dennis     (501) staff       (20)        0 2016-02-16 10:20:45.000000 django-storage-swift-1.2.9/
-drwxr-xr-x   0 dennis     (501) staff       (20)        0 2016-02-16 10:20:45.000000 django-storage-swift-1.2.9/django_storage_swift.egg-info/
--rw-r--r--   0 dennis     (501) staff       (20)        1 2016-02-16 10:20:45.000000 django-storage-swift-1.2.9/django_storage_swift.egg-info/dependency_links.txt
--rw-r--r--   0 dennis     (501) staff       (20)        1 2015-04-18 13:56:08.000000 django-storage-swift-1.2.9/django_storage_swift.egg-info/not-zip-safe
--rw-r--r--   0 dennis     (501) staff       (20)       47 2015-04-18 13:56:45.000000 django-storage-swift-1.2.9/django_storage_swift.egg-info/pbr.json
--rw-r--r--   0 dennis     (501) staff       (20)    16502 2016-02-16 10:20:45.000000 django-storage-swift-1.2.9/django_storage_swift.egg-info/PKG-INFO
--rw-r--r--   0 dennis     (501) staff       (20)       80 2016-02-16 10:20:45.000000 django-storage-swift-1.2.9/django_storage_swift.egg-info/requires.txt
--rw-r--r--   0 dennis     (501) staff       (20)      377 2016-02-16 10:20:45.000000 django-storage-swift-1.2.9/django_storage_swift.egg-info/SOURCES.txt
--rw-r--r--   0 dennis     (501) staff       (20)        6 2016-02-16 10:20:45.000000 django-storage-swift-1.2.9/django_storage_swift.egg-info/top_level.txt
--rw-r--r--   0 dennis     (501) staff       (20)       19 2015-11-23 16:42:44.000000 django-storage-swift-1.2.9/MANIFEST.in
--rw-r--r--   0 dennis     (501) staff       (20)    16502 2016-02-16 10:20:45.000000 django-storage-swift-1.2.9/PKG-INFO
--rw-r--r--   0 dennis     (501) staff       (20)    13997 2016-02-02 15:31:02.000000 django-storage-swift-1.2.9/README.rst
--rw-r--r--   0 dennis     (501) staff       (20)       88 2016-02-16 10:20:45.000000 django-storage-swift-1.2.9/setup.cfg
--rw-r--r--   0 dennis     (501) staff       (20)     1157 2016-02-16 10:20:13.000000 django-storage-swift-1.2.9/setup.py
-drwxr-xr-x   0 dennis     (501) staff       (20)        0 2016-02-16 10:20:45.000000 django-storage-swift-1.2.9/swift/
--rw-r--r--   0 dennis     (501) staff       (20)        0 2015-03-09 10:44:00.000000 django-storage-swift-1.2.9/swift/__init__.py
--rw-r--r--   0 dennis     (501) staff       (20)    12025 2016-02-02 16:40:50.000000 django-storage-swift-1.2.9/swift/storage.py
+drwxr-xr-x   0 dennis    (1000) dennis    (1000)        0 2023-07-27 19:15:39.473931 django-storage-swift-1.3.0/
+-rw-r--r--   0 dennis    (1000) dennis    (1000)     1069 2023-07-27 19:11:23.000000 django-storage-swift-1.3.0/LICENSE.txt
+-rw-r--r--   0 dennis    (1000) dennis    (1000)       19 2023-07-27 19:11:23.000000 django-storage-swift-1.3.0/MANIFEST.in
+-rw-r--r--   0 dennis    (1000) dennis    (1000)    21918 2023-07-27 19:15:39.473931 django-storage-swift-1.3.0/PKG-INFO
+-rw-r--r--   0 dennis    (1000) dennis    (1000)    21149 2023-07-27 19:11:23.000000 django-storage-swift-1.3.0/README.rst
+drwxr-xr-x   0 dennis    (1000) dennis    (1000)        0 2023-07-27 19:15:39.473931 django-storage-swift-1.3.0/django_storage_swift.egg-info/
+-rw-r--r--   0 dennis    (1000) dennis    (1000)    21918 2023-07-27 19:15:39.000000 django-storage-swift-1.3.0/django_storage_swift.egg-info/PKG-INFO
+-rw-r--r--   0 dennis    (1000) dennis    (1000)      365 2023-07-27 19:15:39.000000 django-storage-swift-1.3.0/django_storage_swift.egg-info/SOURCES.txt
+-rw-r--r--   0 dennis    (1000) dennis    (1000)        1 2023-07-27 19:15:39.000000 django-storage-swift-1.3.0/django_storage_swift.egg-info/dependency_links.txt
+-rw-r--r--   0 dennis    (1000) dennis    (1000)        1 2023-07-27 19:14:36.000000 django-storage-swift-1.3.0/django_storage_swift.egg-info/not-zip-safe
+-rw-r--r--   0 dennis    (1000) dennis    (1000)       80 2023-07-27 19:15:39.000000 django-storage-swift-1.3.0/django_storage_swift.egg-info/requires.txt
+-rw-r--r--   0 dennis    (1000) dennis    (1000)        6 2023-07-27 19:15:39.000000 django-storage-swift-1.3.0/django_storage_swift.egg-info/top_level.txt
+-rw-r--r--   0 dennis    (1000) dennis    (1000)       67 2023-07-27 19:15:39.473931 django-storage-swift-1.3.0/setup.cfg
+-rw-r--r--   0 dennis    (1000) dennis    (1000)     1060 2023-07-27 19:15:33.000000 django-storage-swift-1.3.0/setup.py
+drwxr-xr-x   0 dennis    (1000) dennis    (1000)        0 2023-07-27 19:15:39.473931 django-storage-swift-1.3.0/swift/
+-rw-r--r--   0 dennis    (1000) dennis    (1000)        0 2023-07-27 19:11:23.000000 django-storage-swift-1.3.0/swift/__init__.py
+-rw-r--r--   0 dennis    (1000) dennis    (1000)    17316 2023-07-27 19:11:23.000000 django-storage-swift-1.3.0/swift/storage.py
+drwxr-xr-x   0 dennis    (1000) dennis    (1000)        0 2023-07-27 19:15:39.473931 django-storage-swift-1.3.0/tests/
+-rw-r--r--   0 dennis    (1000) dennis    (1000)    18611 2023-07-27 19:11:23.000000 django-storage-swift-1.3.0/tests/tests.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-storage-swift-1.2.9/django_storage_swift.egg-info/PKG-INFO` & `django-storage-swift-1.3.0/README.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,226 +1,248 @@
-Metadata-Version: 1.1
-Name: django-storage-swift
-Version: 1.2.9
-Summary: OpenStack Swift storage backend for Django
-Home-page: http://github.com/blacktorn/django-storage-swift
-Author: Dennis Vermeulen
-Author-email: blacktorn@gmail.com
-License: MIT
-Description: django-storage-swift: a storage layer for OpenStack Swift
-        =========================================================
-        
-        django-storage-swift allows Django applications to use OpenStack Swift
-        as a file storage layer.
-        
-        Features
-        --------
-        
-        -  Reads/writes files into/out of Swift.
-        -  Automatically derives the correct URL to allow files to be accessed
-           through a web browser based on information returned from the
-           authorisation server.
-        
-           -  Allows you to override the host, port and path as necessary.
-           -  Supports the generation of temporary URLs to restrict access to
-              files.
-        
-        Usage
-        -----
-        
-        You can install django-storage-swift through pip. To store your media
-        files on swift, add the following line to your settings.py or
-        local\_settings.py:
-        
-        .. code:: python
-        
-            DEFAULT_FILE_STORAGE='swift.storage.SwiftStorage'
-        
-        To store your static files on swift, add the following line:
-        
-        .. code:: python
-        
-            STATICFILES_STORAGE ='swift.storage.StaticSwiftStorage'
-        
-        This will use another container.
-        
-        Configuring
-        -----------
-        
-        django-storage-swift recognises the following options.
-        
-        +----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-        | Option                                       | Default   | Description                                                                                                                                        |
-        +==============================================+===========+====================================================================================================================================================+
-        | ``SWIFT_AUTH_URL``                           | None      | The URL for the auth server, e.g. ``http://127.0.0.1:5000/v2.0``                                                                                   |
-        +----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-        | ``SWIFT_USERNAME``                           | None      | The username to use to authenticate.                                                                                                               |
-        +----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-        | ``SWIFT_KEY``                                | None      | The key (password) to use to authenticate.                                                                                                         |
-        +----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-        | ``SWIFT_AUTH_VERSION``                       | 1         | The version of the authentication protocol to use.                                                                                                 |
-        +----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-        | ``SWIFT_TENANT_NAME``                        | None      | The tenant name to use when authenticating.                                                                                                        |
-        +----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-        | ``SWIFT_TENANT_ID``                          | None      | The tenant id to use when authenticating.                                                                                                          |
-        +----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-        | ``SWIFT_CONTAINER_NAME``                     | None      | The container in which to store the files.                                                                                                         |
-        +----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-        | ``SWIFT_STATIC_CONTAINER_NAME``              | None      | Alternate container used by StaticSwiftStorage.                                                                                                    |
-        +----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-        | ``SWIFT_AUTO_CREATE_CONTAINER``              | False     | Should the container be created if it does not exist?                                                                                              |
-        +----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-        | ``SWIFT_AUTO_CREATE_CONTAINER_ALLOW_ORIGIN`` | None      | Set the container's X-Container-Meta-Access-Control-Allow-Origin value, to support CORS requests.                                                  |
-        +----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-        | ``SWIFT_AUTO_BASE_URL``                      | True      | Query the authentication server for the base URL.                                                                                                  |
-        +----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-        | ``SWIFT_BASE_URL``                           | None      | The base URL from which the files can be retrieved, e.g. ``http://127.0.0.1:8080/``.                                                               |
-        +----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-        | ``SWIFT_NAME_PREFIX``                        | None      | Prefix that gets added to all filenames.                                                                                                           |
-        +----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-        | ``SWIFT_USE_TEMP_URLS``                      | False     | Generate temporary URLs for file access (allows files to be accessed without a permissive ACL).                                                    |
-        +----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-        | ``SWIFT_TEMP_URL_KEY``                       | None      | Temporary URL key --- see `the OpenStack documentation <http://docs.openstack.org/trunk/config-reference/content//object-storage-tempurl.html>`__. |
-        +----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-        | ``SWIFT_TEMP_URL_DURATION``                  | ``30*60`` | How long a temporary URL remains valid, in seconds.                                                                                                |
-        +----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-        | ``SWIFT_EXTRA_OPTIONS``                      | ``{}``    | Extra options, eg. { "endpoint\_type": "adminURL" }, which will return adminURL instead publicURL.                                                 |
-        +----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-        | ``SWIFT_STATIC_BASE_URL``                    | None      | The base URL from which the static files can be retrieved, e.g. ``http://127.0.0.1:8080/``.                                                        |
-        +----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-        | ``SWIFT_STATIC_NAME_PREFIX``                 | None      | Prefix that gets added to all static filenames.                                                                                                    |
-        +----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-        | ``SWIFT_CONTENT_TYPE_FROM_FD``               | False     | Determine the files mimetypes from the actual content rather than from their filename (default).                                                   |
-        +----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-        
-        SWIFT\_BASE\_URL
-        ~~~~~~~~~~~~~~~~
-        
-        django-swift-storage will automatically query the authentication server
-        for the URL where your files can be accessed, which takes the form
-        ``http://server:port/v1/AUTH_token/``.
-        
-        Sometimes you want to override the server and port (for example if
-        you're developing using `devstack <http://devstack.org/>`__ inside
-        Vagrant). This can be accomplished with ``SWIFT_BASE_URL``.
-        
-        The provided value is parsed, and:
-        
-        -  host and port override any automatically derived values
-        -  any path component is put before derived path components.
-        
-        So if your auth server returns
-        ``http://10.0.2.2:8080/v1/AUTH_012345abcd/`` and you have
-        ``SWIFT_BASE_URL="http://127.0.0.1:8888/foo"``, the ``url`` function
-        will a path based on ``http://127.0.0.1:8888/foo/v1/AUTH_012345abcd/``.
-        
-        Temporary URLs
-        ~~~~~~~~~~~~~~
-        
-        Temporary URLs provide a means to grant a user permission to access a
-        file for a limited time only and without making the entire container
-        public.
-        
-        Temporary URLs work as described in the Swift documentation. (The code
-        to generate the signatures is heavily based on their implementation.)
-        They require setup of a key for signing: the process is described in
-        `the OpenStack
-        documentation <http://docs.openstack.org/trunk/config-reference/content//object-storage-tempurl.html>`__.
-        
-        Use
-        ---
-        
-        Once installed and configured, use of django-storage-swift should be
-        automatic and seamless.
-        
-        You can verify that swift is indeed being used by running, inside
-        ``python manage.py shell``:
-        
-        .. code:: python
-        
-            from django.core.files.storage import default_storage
-            default_storage.connection
-        
-        The result should be ``<<swiftclient.client.Connection object ...>>``
-        
-        Openstack Keystone/Identity v3
-        ------------------------------
-        
-        To authenticate with a swift installation using Keystone AUTH and the Identity v3 API, you must also specify either the domain ID or name that your user and project (tenant) belongs to.
-        
-        .. code:: python
-        
-            SWIFT_AUTH_URL='https://keystoneserver/v3'
-            SWIFT_AUTH_VERSION='3'
-            SWIFT_USERNAME='<<USERNAME>>'
-            SWIFT_KEY='<<PASSWORD>>'
-            SWIFT_TENANT_NAME='<<TENANT_NAME>>'
-            SWIFT_USER_DOMAIN_NAME='<<DOMAIN_NAME>>'
-            SWIFT_PROJECT_DOMAIN_NAME='<<DOMAIN_NAME>>'
-        
-        Troubleshooting
-        ---------------
-        
-        -  **I'm getting permission errors accessing my files**: If you are not
-           using temporary URLs, you may need to make the container publically
-           readable. See `this helpful
-           discussion <http://support.rc.nectar.org.au/forum/viewtopic.php?f=6&t=272>`__.
-           If you are using temporary URLs, verify that your key is set
-           correctly.
-        
-        Quickstart
-        ----------
-        
-        .. code:: python
-        
-            # This was executed on a VM running a SAIO, for example with
-            # https://github.com/swiftstack/vagrant-swift-all-in-one
-        
-            # Create two world-readable containers
-            swift post -r ".r:*" django
-            swift post -r ".r:*" django-static
-        
-            # A virtualenv to keep installation separated
-            virtualenv sampleenv
-            source sampleenv/bin/activate
-            pip install django-storage-swift
-            pip install django
-        
-            # Create a sample project
-            django-admin startproject sampleproj
-            export DJANGO_SETTINGS_MODULE=sampleproj.settings
-            cd sampleproj/
-        
-            # A few required settings, using SAIO defaults
-            cat <<EOF >> sampleproj/settings.py
-            DEFAULT_FILE_STORAGE='swift.storage.SwiftStorage'
-            STATICFILES_STORAGE ='swift.storage.StaticSwiftStorage'
-            SWIFT_AUTH_URL='http://127.0.0.1:8080/auth/v1.0'
-            SWIFT_USERNAME='test:tester'
-            SWIFT_KEY='testing'
-            SWIFT_CONTAINER_NAME='django'
-            SWIFT_STATIC_CONTAINER_NAME='django-static'
-            EOF
-        
-            # Create the initial DB data
-            python manage.py migrate
-        
-            # This uploads static files to Swift
-            python manage.py collectstatic --noinput
-        
-            # Now open http://127.0.0.1:8000/admin/ in your browser
-            # Static files like CSS are served by Swift
-            python manage.py runserver
-        
-Platform: UNKNOWN
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+.. image:: https://img.shields.io/pypi/v/django-storage-swift.svg
+    :target: https://pypi.python.org/pypi/django-storage-swift
+
+.. image:: https://travis-ci.org/dennisv/django-storage-swift.svg?branch=master
+    :target: https://travis-ci.org/dennisv/django-storage-swift
+
+.. image:: https://codecov.io/gh/dennisv/django-storage-swift/branch/master/graph/badge.svg
+   :target: https://codecov.io/gh/dennisv/django-storage-swift
+
+django-storage-swift: a storage layer for OpenStack Swift
+=========================================================
+
+django-storage-swift allows Django applications to use OpenStack Swift
+as a file storage layer.
+
+Features
+--------
+
+-  Reads/writes files into/out of Swift.
+-  Automatically derives the correct URL to allow files to be accessed
+   through a web browser based on information returned from the
+   authorisation server.
+
+   -  Allows you to override the host, port and path as necessary.
+   -  Supports the generation of temporary URLs to restrict access to
+      files.
+
+Usage
+-----
+
+You can install django-storage-swift through pip. To store your media
+files on swift, add the following line to your settings.py or
+local\_settings.py:
+
+.. code:: python
+
+    DEFAULT_FILE_STORAGE = 'swift.storage.SwiftStorage'
+
+To store your static files on swift, add the following line:
+
+.. code:: python
+
+    STATICFILES_STORAGE = 'swift.storage.StaticSwiftStorage'
+
+This will use another container.
+
+Configuring
+-----------
+
+django-storage-swift recognises the following options.
+
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| Option                                       | Default        | Description                                                                                                                                        |
++==============================================+================+====================================================================================================================================================+
+| ``SWIFT_AUTH_URL``                           | *Required*     | The URL for the auth server, e.g. ``http://127.0.0.1:5000/v2.0``                                                                                   |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_USERNAME``                           | *Required*     | The username to use to authenticate.                                                                                                               |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_KEY``/``SWIFT_PASSWORD``             | *Required*     | The key (password) to use to authenticate.                                                                                                         |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_AUTH_VERSION``                       | None           | The version of the authentication protocol to use. If no auth version is defined, a version will be guessed based on auth parameters.              |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_TENANT_NAME``/``SWIFT_PROJECT_NAME`` | None           | (v2 and v3 auth) The tenant/project name to use when authenticating.                                                                               |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_TENANT_ID``/``SWIFT_PROJECT_ID``     | None           | (v2 and v3 auth) The tenant/project id to use when authenticating.                                                                                 |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_USER_DOMAIN_NAME``                   | None           | (v3 auth only) The domain name we authenticate to                                                                                                  |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_USER_DOMAIN_ID``                     | None           | (v3 auth only) The domain id we authenticate to                                                                                                    |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_PROJECT_DOMAIN_NAME``                | None           | (v3 auth only) The domain name our project is located in                                                                                           |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_PROJECT_DOMAIN_ID``                  | None           | (v3 auth only) The domain id our project is located in                                                                                             |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_REGION_NAME``                        | None           | OpenStack region if needed. Check with your provider.                                                                                              |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_CONTAINER_NAME``                     | None           | The container in which to store the files. (``DEFAULT_FILE_STORAGE``)                                                                              |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_STATIC_CONTAINER_NAME``              | None           | Alternate container for storing staticfiles. (``STATICFILES_STORAGE``)                                                                             |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_AUTO_CREATE_CONTAINER``              | False          | Should the container be created if it does not exist?                                                                                              |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_AUTO_CREATE_CONTAINER_PUBLIC``       | False          | Set the auto created container as public on creation                                                                                               |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_AUTO_CREATE_CONTAINER_ALLOW_ORIGIN`` | None           | Set the container's X-Container-Meta-Access-Control-Allow-Origin value, to support CORS requests.                                                  |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_AUTO_BASE_URL``                      | True           | Query the authentication server for the base URL.                                                                                                  |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_BASE_URL``                           | None           | The base URL from which the files can be retrieved, e.g. ``http://127.0.0.1:8080/``.                                                               |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_NAME_PREFIX``                        | None           | Prefix that gets added to all filenames.                                                                                                           |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_USE_TEMP_URLS``                      | False          | Generate temporary URLs for file access (allows files to be accessed without a permissive ACL).                                                    |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_TEMP_URL_KEY``                       | None           | Temporary URL key --- see `the OpenStack documentation <http://docs.openstack.org/trunk/config-reference/content//object-storage-tempurl.html>`__. |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_TEMP_URL_DURATION``                  | ``30*60``      | How long a temporary URL remains valid, in seconds.                                                                                                |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_EXTRA_OPTIONS``                      | ``{}``         | Extra options, eg. { "endpoint\_type": "adminURL" }, which will return adminURL instead publicURL.                                                 |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_STATIC_AUTO_BASE_URL``               | True           | Query the authentication server for the static base URL.                                                                                           |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_STATIC_BASE_URL``                    | None           | The base URL from which the static files can be retrieved, e.g. ``http://127.0.0.1:8080/``.                                                        |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_STATIC_NAME_PREFIX``                 | None           | Prefix that gets added to all static filenames.                                                                                                    |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_CONTENT_TYPE_FROM_FD``               | False          | Determine the files mimetypes from the actual content rather than from their filename (default).                                                   |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_FULL_LISTING``                       | True           | Ensures to get whole directory contents (by default swiftclient limits it to 10000 entries)                                                        |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_AUTH_TOKEN_DURATION``                | ``60*60*23``   | How long a token is expected to be valid in seconds.                                                                                               |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_LAZY_CONNECT``                       | ``False``      | If ``True`` swift connection will be obtained on first use, if ``False`` it will be obtained during storage instantiation. This can decrease       |
+|                                              |                | startup time if you use many fields that use non-default swift storage.                                                                            |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_GZIP_CONTENT_TYPES``                 | ``[]``         | List of content type that will be compressed eg. ['text/plain', 'application/json']                                                                |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_GZIP_COMPRESSION_LEVEL``             | ``4``          | Gzip compression level from 0 to 9. 0 = no compression, 9 = max compression                                                                        |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_GZIP_UNKNOWN_CONTENT_TYPE``          | ``False``      | If set to True and the content-type can't be guessed, gzip anyway                                                                                  |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_CACHE_HEADERS``                      | False          | Headers cache on/off switcher                                                                                                                      |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+
+
+SWIFT\_BASE\_URL
+~~~~~~~~~~~~~~~~
+
+django-swift-storage will automatically query the authentication server
+for the URL where your files can be accessed, which takes the form
+``http://server:port/v1/AUTH_token/``.
+
+Sometimes you want to override the server and port (for example if
+you're developing using `devstack <http://devstack.org/>`__ inside
+Vagrant). This can be accomplished with ``SWIFT_BASE_URL``.
+
+The provided value is parsed, and:
+
+-  host and port override any automatically derived values
+-  any path component is put before derived path components.
+
+So if your auth server returns
+``http://10.0.2.2:8080/v1/AUTH_012345abcd/`` and you have
+``SWIFT_BASE_URL="http://127.0.0.1:8888/foo"``, the ``url`` function
+will a path based on ``http://127.0.0.1:8888/foo/v1/AUTH_012345abcd/``.
+
+Temporary URLs
+~~~~~~~~~~~~~~
+
+Temporary URLs provide a means to grant a user permission to access a
+file for a limited time only and without making the entire container
+public.
+
+Temporary URLs work as described in the Swift documentation. (The code
+to generate the signatures is heavily based on their implementation.)
+They require setup of a key for signing: the process is described in
+`the OpenStack
+documentation <http://docs.openstack.org/trunk/config-reference/content//object-storage-tempurl.html>`__.
+
+Use
+---
+
+Once installed and configured, use of django-storage-swift should be
+automatic and seamless.
+
+You can verify that swift is indeed being used by running, inside
+``python manage.py shell``:
+
+.. code:: python
+
+    from django.core.files.storage import default_storage
+    default_storage.http_conn
+
+The result should be ``<<swiftclient.client.Connection object ...>>``
+
+Openstack Keystone/Identity v3
+------------------------------
+
+To authenticate with a swift installation using Keystone AUTH and the Identity v3 API, you must also specify either the domain ID or name that your user and project (tenant) belongs to.
+
+.. code:: python
+
+    SWIFT_AUTH_URL='https://keystoneserver/v3'
+    SWIFT_AUTH_VERSION='3'
+    SWIFT_USERNAME='<<USERNAME>>'
+    SWIFT_KEY='<<PASSWORD>>'
+    SWIFT_TENANT_NAME='<<TENANT_NAME>>'
+    SWIFT_USER_DOMAIN_NAME='<<DOMAIN_NAME>>'
+    SWIFT_PROJECT_DOMAIN_NAME='<<DOMAIN_NAME>>'
+
+Troubleshooting
+---------------
+
+-  **I'm getting permission errors accessing my files**: If you are not
+   using temporary URLs, you may need to make the container publically
+   readable. See `this helpful
+   discussion <http://support.rc.nectar.org.au/forum/viewtopic.php?f=6&t=272>`__.
+   If you are using temporary URLs, verify that your key is set
+   correctly.
+-  **I'm getting empty or truncated file uploads**: Issues with some content
+   types may cause an incorrect `content_length` header to be sent with file
+   uploads, resulting in 0 byte or truncated files.  To avoid this, set
+   `SWIFT_CONTENT_LENGTH_FROM_FD: True`.
+
+
+Quickstart
+----------
+
+.. code:: python
+
+    # This was executed on a VM running a SAIO, for example with
+    # https://github.com/swiftstack/vagrant-swift-all-in-one
+
+    # Create two world-readable containers
+    swift post -r ".r:*" django
+    swift post -r ".r:*" django-static
+
+    # A virtualenv to keep installation separated
+    virtualenv sampleenv
+    source sampleenv/bin/activate
+    pip install django-storage-swift
+    pip install django
+
+    # Create a sample project
+    django-admin startproject sampleproj
+    export DJANGO_SETTINGS_MODULE=sampleproj.settings
+    cd sampleproj/
+
+    # A few required settings, using SAIO defaults
+    cat <<EOF >> sampleproj/settings.py
+    DEFAULT_FILE_STORAGE='swift.storage.SwiftStorage'
+    STATICFILES_STORAGE ='swift.storage.StaticSwiftStorage'
+    SWIFT_AUTH_URL='http://127.0.0.1:8080/auth/v1.0'
+    SWIFT_USERNAME='test:tester'
+    SWIFT_KEY='testing'
+    SWIFT_CONTAINER_NAME='django'
+    SWIFT_STATIC_CONTAINER_NAME='django-static'
+    EOF
+
+    # Create the initial DB data
+    python manage.py migrate
+
+    # This uploads static files to Swift
+    python manage.py collectstatic --noinput
+
+    # Now open http://127.0.0.1:8000/admin/ in your browser
+    # Static files like CSS are served by Swift
+    python manage.py runserver
```

### Comparing `django-storage-swift-1.2.9/PKG-INFO` & `django-storage-swift-1.3.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,226 +1,268 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: django-storage-swift
-Version: 1.2.9
+Version: 1.3.0
 Summary: OpenStack Swift storage backend for Django
-Home-page: http://github.com/blacktorn/django-storage-swift
+Home-page: https://github.com/dennisv/django-storage-swift
 Author: Dennis Vermeulen
 Author-email: blacktorn@gmail.com
 License: MIT
-Description: django-storage-swift: a storage layer for OpenStack Swift
-        =========================================================
-        
-        django-storage-swift allows Django applications to use OpenStack Swift
-        as a file storage layer.
-        
-        Features
-        --------
-        
-        -  Reads/writes files into/out of Swift.
-        -  Automatically derives the correct URL to allow files to be accessed
-           through a web browser based on information returned from the
-           authorisation server.
-        
-           -  Allows you to override the host, port and path as necessary.
-           -  Supports the generation of temporary URLs to restrict access to
-              files.
-        
-        Usage
-        -----
-        
-        You can install django-storage-swift through pip. To store your media
-        files on swift, add the following line to your settings.py or
-        local\_settings.py:
-        
-        .. code:: python
-        
-            DEFAULT_FILE_STORAGE='swift.storage.SwiftStorage'
-        
-        To store your static files on swift, add the following line:
-        
-        .. code:: python
-        
-            STATICFILES_STORAGE ='swift.storage.StaticSwiftStorage'
-        
-        This will use another container.
-        
-        Configuring
-        -----------
-        
-        django-storage-swift recognises the following options.
-        
-        +----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-        | Option                                       | Default   | Description                                                                                                                                        |
-        +==============================================+===========+====================================================================================================================================================+
-        | ``SWIFT_AUTH_URL``                           | None      | The URL for the auth server, e.g. ``http://127.0.0.1:5000/v2.0``                                                                                   |
-        +----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-        | ``SWIFT_USERNAME``                           | None      | The username to use to authenticate.                                                                                                               |
-        +----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-        | ``SWIFT_KEY``                                | None      | The key (password) to use to authenticate.                                                                                                         |
-        +----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-        | ``SWIFT_AUTH_VERSION``                       | 1         | The version of the authentication protocol to use.                                                                                                 |
-        +----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-        | ``SWIFT_TENANT_NAME``                        | None      | The tenant name to use when authenticating.                                                                                                        |
-        +----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-        | ``SWIFT_TENANT_ID``                          | None      | The tenant id to use when authenticating.                                                                                                          |
-        +----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-        | ``SWIFT_CONTAINER_NAME``                     | None      | The container in which to store the files.                                                                                                         |
-        +----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-        | ``SWIFT_STATIC_CONTAINER_NAME``              | None      | Alternate container used by StaticSwiftStorage.                                                                                                    |
-        +----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-        | ``SWIFT_AUTO_CREATE_CONTAINER``              | False     | Should the container be created if it does not exist?                                                                                              |
-        +----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-        | ``SWIFT_AUTO_CREATE_CONTAINER_ALLOW_ORIGIN`` | None      | Set the container's X-Container-Meta-Access-Control-Allow-Origin value, to support CORS requests.                                                  |
-        +----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-        | ``SWIFT_AUTO_BASE_URL``                      | True      | Query the authentication server for the base URL.                                                                                                  |
-        +----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-        | ``SWIFT_BASE_URL``                           | None      | The base URL from which the files can be retrieved, e.g. ``http://127.0.0.1:8080/``.                                                               |
-        +----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-        | ``SWIFT_NAME_PREFIX``                        | None      | Prefix that gets added to all filenames.                                                                                                           |
-        +----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-        | ``SWIFT_USE_TEMP_URLS``                      | False     | Generate temporary URLs for file access (allows files to be accessed without a permissive ACL).                                                    |
-        +----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-        | ``SWIFT_TEMP_URL_KEY``                       | None      | Temporary URL key --- see `the OpenStack documentation <http://docs.openstack.org/trunk/config-reference/content//object-storage-tempurl.html>`__. |
-        +----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-        | ``SWIFT_TEMP_URL_DURATION``                  | ``30*60`` | How long a temporary URL remains valid, in seconds.                                                                                                |
-        +----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-        | ``SWIFT_EXTRA_OPTIONS``                      | ``{}``    | Extra options, eg. { "endpoint\_type": "adminURL" }, which will return adminURL instead publicURL.                                                 |
-        +----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-        | ``SWIFT_STATIC_BASE_URL``                    | None      | The base URL from which the static files can be retrieved, e.g. ``http://127.0.0.1:8080/``.                                                        |
-        +----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-        | ``SWIFT_STATIC_NAME_PREFIX``                 | None      | Prefix that gets added to all static filenames.                                                                                                    |
-        +----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-        | ``SWIFT_CONTENT_TYPE_FROM_FD``               | False     | Determine the files mimetypes from the actual content rather than from their filename (default).                                                   |
-        +----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-        
-        SWIFT\_BASE\_URL
-        ~~~~~~~~~~~~~~~~
-        
-        django-swift-storage will automatically query the authentication server
-        for the URL where your files can be accessed, which takes the form
-        ``http://server:port/v1/AUTH_token/``.
-        
-        Sometimes you want to override the server and port (for example if
-        you're developing using `devstack <http://devstack.org/>`__ inside
-        Vagrant). This can be accomplished with ``SWIFT_BASE_URL``.
-        
-        The provided value is parsed, and:
-        
-        -  host and port override any automatically derived values
-        -  any path component is put before derived path components.
-        
-        So if your auth server returns
-        ``http://10.0.2.2:8080/v1/AUTH_012345abcd/`` and you have
-        ``SWIFT_BASE_URL="http://127.0.0.1:8888/foo"``, the ``url`` function
-        will a path based on ``http://127.0.0.1:8888/foo/v1/AUTH_012345abcd/``.
-        
-        Temporary URLs
-        ~~~~~~~~~~~~~~
-        
-        Temporary URLs provide a means to grant a user permission to access a
-        file for a limited time only and without making the entire container
-        public.
-        
-        Temporary URLs work as described in the Swift documentation. (The code
-        to generate the signatures is heavily based on their implementation.)
-        They require setup of a key for signing: the process is described in
-        `the OpenStack
-        documentation <http://docs.openstack.org/trunk/config-reference/content//object-storage-tempurl.html>`__.
-        
-        Use
-        ---
-        
-        Once installed and configured, use of django-storage-swift should be
-        automatic and seamless.
-        
-        You can verify that swift is indeed being used by running, inside
-        ``python manage.py shell``:
-        
-        .. code:: python
-        
-            from django.core.files.storage import default_storage
-            default_storage.connection
-        
-        The result should be ``<<swiftclient.client.Connection object ...>>``
-        
-        Openstack Keystone/Identity v3
-        ------------------------------
-        
-        To authenticate with a swift installation using Keystone AUTH and the Identity v3 API, you must also specify either the domain ID or name that your user and project (tenant) belongs to.
-        
-        .. code:: python
-        
-            SWIFT_AUTH_URL='https://keystoneserver/v3'
-            SWIFT_AUTH_VERSION='3'
-            SWIFT_USERNAME='<<USERNAME>>'
-            SWIFT_KEY='<<PASSWORD>>'
-            SWIFT_TENANT_NAME='<<TENANT_NAME>>'
-            SWIFT_USER_DOMAIN_NAME='<<DOMAIN_NAME>>'
-            SWIFT_PROJECT_DOMAIN_NAME='<<DOMAIN_NAME>>'
-        
-        Troubleshooting
-        ---------------
-        
-        -  **I'm getting permission errors accessing my files**: If you are not
-           using temporary URLs, you may need to make the container publically
-           readable. See `this helpful
-           discussion <http://support.rc.nectar.org.au/forum/viewtopic.php?f=6&t=272>`__.
-           If you are using temporary URLs, verify that your key is set
-           correctly.
-        
-        Quickstart
-        ----------
-        
-        .. code:: python
-        
-            # This was executed on a VM running a SAIO, for example with
-            # https://github.com/swiftstack/vagrant-swift-all-in-one
-        
-            # Create two world-readable containers
-            swift post -r ".r:*" django
-            swift post -r ".r:*" django-static
-        
-            # A virtualenv to keep installation separated
-            virtualenv sampleenv
-            source sampleenv/bin/activate
-            pip install django-storage-swift
-            pip install django
-        
-            # Create a sample project
-            django-admin startproject sampleproj
-            export DJANGO_SETTINGS_MODULE=sampleproj.settings
-            cd sampleproj/
-        
-            # A few required settings, using SAIO defaults
-            cat <<EOF >> sampleproj/settings.py
-            DEFAULT_FILE_STORAGE='swift.storage.SwiftStorage'
-            STATICFILES_STORAGE ='swift.storage.StaticSwiftStorage'
-            SWIFT_AUTH_URL='http://127.0.0.1:8080/auth/v1.0'
-            SWIFT_USERNAME='test:tester'
-            SWIFT_KEY='testing'
-            SWIFT_CONTAINER_NAME='django'
-            SWIFT_STATIC_CONTAINER_NAME='django-static'
-            EOF
-        
-            # Create the initial DB data
-            python manage.py migrate
-        
-            # This uploads static files to Swift
-            python manage.py collectstatic --noinput
-        
-            # Now open http://127.0.0.1:8000/admin/ in your browser
-            # Static files like CSS are served by Swift
-            python manage.py runserver
-        
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+License-File: LICENSE.txt
+
+.. image:: https://img.shields.io/pypi/v/django-storage-swift.svg
+    :target: https://pypi.python.org/pypi/django-storage-swift
+
+.. image:: https://travis-ci.org/dennisv/django-storage-swift.svg?branch=master
+    :target: https://travis-ci.org/dennisv/django-storage-swift
+
+.. image:: https://codecov.io/gh/dennisv/django-storage-swift/branch/master/graph/badge.svg
+   :target: https://codecov.io/gh/dennisv/django-storage-swift
+
+django-storage-swift: a storage layer for OpenStack Swift
+=========================================================
+
+django-storage-swift allows Django applications to use OpenStack Swift
+as a file storage layer.
+
+Features
+--------
+
+-  Reads/writes files into/out of Swift.
+-  Automatically derives the correct URL to allow files to be accessed
+   through a web browser based on information returned from the
+   authorisation server.
+
+   -  Allows you to override the host, port and path as necessary.
+   -  Supports the generation of temporary URLs to restrict access to
+      files.
+
+Usage
+-----
+
+You can install django-storage-swift through pip. To store your media
+files on swift, add the following line to your settings.py or
+local\_settings.py:
+
+.. code:: python
+
+    DEFAULT_FILE_STORAGE = 'swift.storage.SwiftStorage'
+
+To store your static files on swift, add the following line:
+
+.. code:: python
+
+    STATICFILES_STORAGE = 'swift.storage.StaticSwiftStorage'
+
+This will use another container.
+
+Configuring
+-----------
+
+django-storage-swift recognises the following options.
+
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| Option                                       | Default        | Description                                                                                                                                        |
++==============================================+================+====================================================================================================================================================+
+| ``SWIFT_AUTH_URL``                           | *Required*     | The URL for the auth server, e.g. ``http://127.0.0.1:5000/v2.0``                                                                                   |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_USERNAME``                           | *Required*     | The username to use to authenticate.                                                                                                               |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_KEY``/``SWIFT_PASSWORD``             | *Required*     | The key (password) to use to authenticate.                                                                                                         |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_AUTH_VERSION``                       | None           | The version of the authentication protocol to use. If no auth version is defined, a version will be guessed based on auth parameters.              |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_TENANT_NAME``/``SWIFT_PROJECT_NAME`` | None           | (v2 and v3 auth) The tenant/project name to use when authenticating.                                                                               |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_TENANT_ID``/``SWIFT_PROJECT_ID``     | None           | (v2 and v3 auth) The tenant/project id to use when authenticating.                                                                                 |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_USER_DOMAIN_NAME``                   | None           | (v3 auth only) The domain name we authenticate to                                                                                                  |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_USER_DOMAIN_ID``                     | None           | (v3 auth only) The domain id we authenticate to                                                                                                    |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_PROJECT_DOMAIN_NAME``                | None           | (v3 auth only) The domain name our project is located in                                                                                           |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_PROJECT_DOMAIN_ID``                  | None           | (v3 auth only) The domain id our project is located in                                                                                             |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_REGION_NAME``                        | None           | OpenStack region if needed. Check with your provider.                                                                                              |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_CONTAINER_NAME``                     | None           | The container in which to store the files. (``DEFAULT_FILE_STORAGE``)                                                                              |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_STATIC_CONTAINER_NAME``              | None           | Alternate container for storing staticfiles. (``STATICFILES_STORAGE``)                                                                             |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_AUTO_CREATE_CONTAINER``              | False          | Should the container be created if it does not exist?                                                                                              |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_AUTO_CREATE_CONTAINER_PUBLIC``       | False          | Set the auto created container as public on creation                                                                                               |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_AUTO_CREATE_CONTAINER_ALLOW_ORIGIN`` | None           | Set the container's X-Container-Meta-Access-Control-Allow-Origin value, to support CORS requests.                                                  |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_AUTO_BASE_URL``                      | True           | Query the authentication server for the base URL.                                                                                                  |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_BASE_URL``                           | None           | The base URL from which the files can be retrieved, e.g. ``http://127.0.0.1:8080/``.                                                               |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_NAME_PREFIX``                        | None           | Prefix that gets added to all filenames.                                                                                                           |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_USE_TEMP_URLS``                      | False          | Generate temporary URLs for file access (allows files to be accessed without a permissive ACL).                                                    |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_TEMP_URL_KEY``                       | None           | Temporary URL key --- see `the OpenStack documentation <http://docs.openstack.org/trunk/config-reference/content//object-storage-tempurl.html>`__. |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_TEMP_URL_DURATION``                  | ``30*60``      | How long a temporary URL remains valid, in seconds.                                                                                                |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_EXTRA_OPTIONS``                      | ``{}``         | Extra options, eg. { "endpoint\_type": "adminURL" }, which will return adminURL instead publicURL.                                                 |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_STATIC_AUTO_BASE_URL``               | True           | Query the authentication server for the static base URL.                                                                                           |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_STATIC_BASE_URL``                    | None           | The base URL from which the static files can be retrieved, e.g. ``http://127.0.0.1:8080/``.                                                        |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_STATIC_NAME_PREFIX``                 | None           | Prefix that gets added to all static filenames.                                                                                                    |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_CONTENT_TYPE_FROM_FD``               | False          | Determine the files mimetypes from the actual content rather than from their filename (default).                                                   |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_FULL_LISTING``                       | True           | Ensures to get whole directory contents (by default swiftclient limits it to 10000 entries)                                                        |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_AUTH_TOKEN_DURATION``                | ``60*60*23``   | How long a token is expected to be valid in seconds.                                                                                               |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_LAZY_CONNECT``                       | ``False``      | If ``True`` swift connection will be obtained on first use, if ``False`` it will be obtained during storage instantiation. This can decrease       |
+|                                              |                | startup time if you use many fields that use non-default swift storage.                                                                            |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_GZIP_CONTENT_TYPES``                 | ``[]``         | List of content type that will be compressed eg. ['text/plain', 'application/json']                                                                |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_GZIP_COMPRESSION_LEVEL``             | ``4``          | Gzip compression level from 0 to 9. 0 = no compression, 9 = max compression                                                                        |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_GZIP_UNKNOWN_CONTENT_TYPE``          | ``False``      | If set to True and the content-type can't be guessed, gzip anyway                                                                                  |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_CACHE_HEADERS``                      | False          | Headers cache on/off switcher                                                                                                                      |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+
+
+SWIFT\_BASE\_URL
+~~~~~~~~~~~~~~~~
+
+django-swift-storage will automatically query the authentication server
+for the URL where your files can be accessed, which takes the form
+``http://server:port/v1/AUTH_token/``.
+
+Sometimes you want to override the server and port (for example if
+you're developing using `devstack <http://devstack.org/>`__ inside
+Vagrant). This can be accomplished with ``SWIFT_BASE_URL``.
+
+The provided value is parsed, and:
+
+-  host and port override any automatically derived values
+-  any path component is put before derived path components.
+
+So if your auth server returns
+``http://10.0.2.2:8080/v1/AUTH_012345abcd/`` and you have
+``SWIFT_BASE_URL="http://127.0.0.1:8888/foo"``, the ``url`` function
+will a path based on ``http://127.0.0.1:8888/foo/v1/AUTH_012345abcd/``.
+
+Temporary URLs
+~~~~~~~~~~~~~~
+
+Temporary URLs provide a means to grant a user permission to access a
+file for a limited time only and without making the entire container
+public.
+
+Temporary URLs work as described in the Swift documentation. (The code
+to generate the signatures is heavily based on their implementation.)
+They require setup of a key for signing: the process is described in
+`the OpenStack
+documentation <http://docs.openstack.org/trunk/config-reference/content//object-storage-tempurl.html>`__.
+
+Use
+---
+
+Once installed and configured, use of django-storage-swift should be
+automatic and seamless.
+
+You can verify that swift is indeed being used by running, inside
+``python manage.py shell``:
+
+.. code:: python
+
+    from django.core.files.storage import default_storage
+    default_storage.http_conn
+
+The result should be ``<<swiftclient.client.Connection object ...>>``
+
+Openstack Keystone/Identity v3
+------------------------------
+
+To authenticate with a swift installation using Keystone AUTH and the Identity v3 API, you must also specify either the domain ID or name that your user and project (tenant) belongs to.
+
+.. code:: python
+
+    SWIFT_AUTH_URL='https://keystoneserver/v3'
+    SWIFT_AUTH_VERSION='3'
+    SWIFT_USERNAME='<<USERNAME>>'
+    SWIFT_KEY='<<PASSWORD>>'
+    SWIFT_TENANT_NAME='<<TENANT_NAME>>'
+    SWIFT_USER_DOMAIN_NAME='<<DOMAIN_NAME>>'
+    SWIFT_PROJECT_DOMAIN_NAME='<<DOMAIN_NAME>>'
+
+Troubleshooting
+---------------
+
+-  **I'm getting permission errors accessing my files**: If you are not
+   using temporary URLs, you may need to make the container publically
+   readable. See `this helpful
+   discussion <http://support.rc.nectar.org.au/forum/viewtopic.php?f=6&t=272>`__.
+   If you are using temporary URLs, verify that your key is set
+   correctly.
+-  **I'm getting empty or truncated file uploads**: Issues with some content
+   types may cause an incorrect `content_length` header to be sent with file
+   uploads, resulting in 0 byte or truncated files.  To avoid this, set
+   `SWIFT_CONTENT_LENGTH_FROM_FD: True`.
+
+
+Quickstart
+----------
+
+.. code:: python
+
+    # This was executed on a VM running a SAIO, for example with
+    # https://github.com/swiftstack/vagrant-swift-all-in-one
+
+    # Create two world-readable containers
+    swift post -r ".r:*" django
+    swift post -r ".r:*" django-static
+
+    # A virtualenv to keep installation separated
+    virtualenv sampleenv
+    source sampleenv/bin/activate
+    pip install django-storage-swift
+    pip install django
+
+    # Create a sample project
+    django-admin startproject sampleproj
+    export DJANGO_SETTINGS_MODULE=sampleproj.settings
+    cd sampleproj/
+
+    # A few required settings, using SAIO defaults
+    cat <<EOF >> sampleproj/settings.py
+    DEFAULT_FILE_STORAGE='swift.storage.SwiftStorage'
+    STATICFILES_STORAGE ='swift.storage.StaticSwiftStorage'
+    SWIFT_AUTH_URL='http://127.0.0.1:8080/auth/v1.0'
+    SWIFT_USERNAME='test:tester'
+    SWIFT_KEY='testing'
+    SWIFT_CONTAINER_NAME='django'
+    SWIFT_STATIC_CONTAINER_NAME='django-static'
+    EOF
+
+    # Create the initial DB data
+    python manage.py migrate
+
+    # This uploads static files to Swift
+    python manage.py collectstatic --noinput
+
+    # Now open http://127.0.0.1:8000/admin/ in your browser
+    # Static files like CSS are served by Swift
+    python manage.py runserver
```

### Comparing `django-storage-swift-1.2.9/README.rst` & `django-storage-swift-1.3.0/django_storage_swift.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,36 @@
+Metadata-Version: 2.1
+Name: django-storage-swift
+Version: 1.3.0
+Summary: OpenStack Swift storage backend for Django
+Home-page: https://github.com/dennisv/django-storage-swift
+Author: Dennis Vermeulen
+Author-email: blacktorn@gmail.com
+License: MIT
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Django
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+License-File: LICENSE.txt
+
+.. image:: https://img.shields.io/pypi/v/django-storage-swift.svg
+    :target: https://pypi.python.org/pypi/django-storage-swift
+
+.. image:: https://travis-ci.org/dennisv/django-storage-swift.svg?branch=master
+    :target: https://travis-ci.org/dennisv/django-storage-swift
+
+.. image:: https://codecov.io/gh/dennisv/django-storage-swift/branch/master/graph/badge.svg
+   :target: https://codecov.io/gh/dennisv/django-storage-swift
+
 django-storage-swift: a storage layer for OpenStack Swift
 =========================================================
 
 django-storage-swift allows Django applications to use OpenStack Swift
 as a file storage layer.
 
 Features
@@ -21,72 +50,102 @@
 
 You can install django-storage-swift through pip. To store your media
 files on swift, add the following line to your settings.py or
 local\_settings.py:
 
 .. code:: python
 
-    DEFAULT_FILE_STORAGE='swift.storage.SwiftStorage'
+    DEFAULT_FILE_STORAGE = 'swift.storage.SwiftStorage'
 
 To store your static files on swift, add the following line:
 
 .. code:: python
 
-    STATICFILES_STORAGE ='swift.storage.StaticSwiftStorage'
+    STATICFILES_STORAGE = 'swift.storage.StaticSwiftStorage'
 
 This will use another container.
 
 Configuring
 -----------
 
 django-storage-swift recognises the following options.
 
-+----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-| Option                                       | Default   | Description                                                                                                                                        |
-+==============================================+===========+====================================================================================================================================================+
-| ``SWIFT_AUTH_URL``                           | None      | The URL for the auth server, e.g. ``http://127.0.0.1:5000/v2.0``                                                                                   |
-+----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-| ``SWIFT_USERNAME``                           | None      | The username to use to authenticate.                                                                                                               |
-+----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-| ``SWIFT_KEY``                                | None      | The key (password) to use to authenticate.                                                                                                         |
-+----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-| ``SWIFT_AUTH_VERSION``                       | 1         | The version of the authentication protocol to use.                                                                                                 |
-+----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-| ``SWIFT_TENANT_NAME``                        | None      | The tenant name to use when authenticating.                                                                                                        |
-+----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-| ``SWIFT_TENANT_ID``                          | None      | The tenant id to use when authenticating.                                                                                                          |
-+----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-| ``SWIFT_CONTAINER_NAME``                     | None      | The container in which to store the files.                                                                                                         |
-+----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-| ``SWIFT_STATIC_CONTAINER_NAME``              | None      | Alternate container used by StaticSwiftStorage.                                                                                                    |
-+----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-| ``SWIFT_AUTO_CREATE_CONTAINER``              | False     | Should the container be created if it does not exist?                                                                                              |
-+----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-| ``SWIFT_AUTO_CREATE_CONTAINER_ALLOW_ORIGIN`` | None      | Set the container's X-Container-Meta-Access-Control-Allow-Origin value, to support CORS requests.                                                  |
-+----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-| ``SWIFT_AUTO_BASE_URL``                      | True      | Query the authentication server for the base URL.                                                                                                  |
-+----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-| ``SWIFT_BASE_URL``                           | None      | The base URL from which the files can be retrieved, e.g. ``http://127.0.0.1:8080/``.                                                               |
-+----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-| ``SWIFT_NAME_PREFIX``                        | None      | Prefix that gets added to all filenames.                                                                                                           |
-+----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-| ``SWIFT_USE_TEMP_URLS``                      | False     | Generate temporary URLs for file access (allows files to be accessed without a permissive ACL).                                                    |
-+----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-| ``SWIFT_TEMP_URL_KEY``                       | None      | Temporary URL key --- see `the OpenStack documentation <http://docs.openstack.org/trunk/config-reference/content//object-storage-tempurl.html>`__. |
-+----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-| ``SWIFT_TEMP_URL_DURATION``                  | ``30*60`` | How long a temporary URL remains valid, in seconds.                                                                                                |
-+----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-| ``SWIFT_EXTRA_OPTIONS``                      | ``{}``    | Extra options, eg. { "endpoint\_type": "adminURL" }, which will return adminURL instead publicURL.                                                 |
-+----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-| ``SWIFT_STATIC_BASE_URL``                    | None      | The base URL from which the static files can be retrieved, e.g. ``http://127.0.0.1:8080/``.                                                        |
-+----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-| ``SWIFT_STATIC_NAME_PREFIX``                 | None      | Prefix that gets added to all static filenames.                                                                                                    |
-+----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
-| ``SWIFT_CONTENT_TYPE_FROM_FD``               | False     | Determine the files mimetypes from the actual content rather than from their filename (default).                                                   |
-+----------------------------------------------+-----------+----------------------------------------------------------------------------------------------------------------------------------------------------+
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| Option                                       | Default        | Description                                                                                                                                        |
++==============================================+================+====================================================================================================================================================+
+| ``SWIFT_AUTH_URL``                           | *Required*     | The URL for the auth server, e.g. ``http://127.0.0.1:5000/v2.0``                                                                                   |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_USERNAME``                           | *Required*     | The username to use to authenticate.                                                                                                               |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_KEY``/``SWIFT_PASSWORD``             | *Required*     | The key (password) to use to authenticate.                                                                                                         |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_AUTH_VERSION``                       | None           | The version of the authentication protocol to use. If no auth version is defined, a version will be guessed based on auth parameters.              |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_TENANT_NAME``/``SWIFT_PROJECT_NAME`` | None           | (v2 and v3 auth) The tenant/project name to use when authenticating.                                                                               |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_TENANT_ID``/``SWIFT_PROJECT_ID``     | None           | (v2 and v3 auth) The tenant/project id to use when authenticating.                                                                                 |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_USER_DOMAIN_NAME``                   | None           | (v3 auth only) The domain name we authenticate to                                                                                                  |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_USER_DOMAIN_ID``                     | None           | (v3 auth only) The domain id we authenticate to                                                                                                    |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_PROJECT_DOMAIN_NAME``                | None           | (v3 auth only) The domain name our project is located in                                                                                           |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_PROJECT_DOMAIN_ID``                  | None           | (v3 auth only) The domain id our project is located in                                                                                             |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_REGION_NAME``                        | None           | OpenStack region if needed. Check with your provider.                                                                                              |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_CONTAINER_NAME``                     | None           | The container in which to store the files. (``DEFAULT_FILE_STORAGE``)                                                                              |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_STATIC_CONTAINER_NAME``              | None           | Alternate container for storing staticfiles. (``STATICFILES_STORAGE``)                                                                             |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_AUTO_CREATE_CONTAINER``              | False          | Should the container be created if it does not exist?                                                                                              |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_AUTO_CREATE_CONTAINER_PUBLIC``       | False          | Set the auto created container as public on creation                                                                                               |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_AUTO_CREATE_CONTAINER_ALLOW_ORIGIN`` | None           | Set the container's X-Container-Meta-Access-Control-Allow-Origin value, to support CORS requests.                                                  |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_AUTO_BASE_URL``                      | True           | Query the authentication server for the base URL.                                                                                                  |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_BASE_URL``                           | None           | The base URL from which the files can be retrieved, e.g. ``http://127.0.0.1:8080/``.                                                               |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_NAME_PREFIX``                        | None           | Prefix that gets added to all filenames.                                                                                                           |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_USE_TEMP_URLS``                      | False          | Generate temporary URLs for file access (allows files to be accessed without a permissive ACL).                                                    |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_TEMP_URL_KEY``                       | None           | Temporary URL key --- see `the OpenStack documentation <http://docs.openstack.org/trunk/config-reference/content//object-storage-tempurl.html>`__. |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_TEMP_URL_DURATION``                  | ``30*60``      | How long a temporary URL remains valid, in seconds.                                                                                                |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_EXTRA_OPTIONS``                      | ``{}``         | Extra options, eg. { "endpoint\_type": "adminURL" }, which will return adminURL instead publicURL.                                                 |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_STATIC_AUTO_BASE_URL``               | True           | Query the authentication server for the static base URL.                                                                                           |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_STATIC_BASE_URL``                    | None           | The base URL from which the static files can be retrieved, e.g. ``http://127.0.0.1:8080/``.                                                        |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_STATIC_NAME_PREFIX``                 | None           | Prefix that gets added to all static filenames.                                                                                                    |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_CONTENT_TYPE_FROM_FD``               | False          | Determine the files mimetypes from the actual content rather than from their filename (default).                                                   |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_FULL_LISTING``                       | True           | Ensures to get whole directory contents (by default swiftclient limits it to 10000 entries)                                                        |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_AUTH_TOKEN_DURATION``                | ``60*60*23``   | How long a token is expected to be valid in seconds.                                                                                               |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_LAZY_CONNECT``                       | ``False``      | If ``True`` swift connection will be obtained on first use, if ``False`` it will be obtained during storage instantiation. This can decrease       |
+|                                              |                | startup time if you use many fields that use non-default swift storage.                                                                            |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_GZIP_CONTENT_TYPES``                 | ``[]``         | List of content type that will be compressed eg. ['text/plain', 'application/json']                                                                |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_GZIP_COMPRESSION_LEVEL``             | ``4``          | Gzip compression level from 0 to 9. 0 = no compression, 9 = max compression                                                                        |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_GZIP_UNKNOWN_CONTENT_TYPE``          | ``False``      | If set to True and the content-type can't be guessed, gzip anyway                                                                                  |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+| ``SWIFT_CACHE_HEADERS``                      | False          | Headers cache on/off switcher                                                                                                                      |
++----------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------+
+
 
 SWIFT\_BASE\_URL
 ~~~~~~~~~~~~~~~~
 
 django-swift-storage will automatically query the authentication server
 for the URL where your files can be accessed, which takes the form
 ``http://server:port/v1/AUTH_token/``.
@@ -126,15 +185,15 @@
 
 You can verify that swift is indeed being used by running, inside
 ``python manage.py shell``:
 
 .. code:: python
 
     from django.core.files.storage import default_storage
-    default_storage.connection
+    default_storage.http_conn
 
 The result should be ``<<swiftclient.client.Connection object ...>>``
 
 Openstack Keystone/Identity v3
 ------------------------------
 
 To authenticate with a swift installation using Keystone AUTH and the Identity v3 API, you must also specify either the domain ID or name that your user and project (tenant) belongs to.
@@ -154,14 +213,19 @@
 
 -  **I'm getting permission errors accessing my files**: If you are not
    using temporary URLs, you may need to make the container publically
    readable. See `this helpful
    discussion <http://support.rc.nectar.org.au/forum/viewtopic.php?f=6&t=272>`__.
    If you are using temporary URLs, verify that your key is set
    correctly.
+-  **I'm getting empty or truncated file uploads**: Issues with some content
+   types may cause an incorrect `content_length` header to be sent with file
+   uploads, resulting in 0 byte or truncated files.  To avoid this, set
+   `SWIFT_CONTENT_LENGTH_FROM_FD: True`.
+
 
 Quickstart
 ----------
 
 .. code:: python
 
     # This was executed on a VM running a SAIO, for example with
```

### Comparing `django-storage-swift-1.2.9/setup.py` & `django-storage-swift-1.3.0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 from setuptools import setup
 
 setup(
     name='django-storage-swift',
-    version='1.2.9',
+    version='1.3.0',
     description='OpenStack Swift storage backend for Django',
     long_description=open('README.rst').read(),
-    url='http://github.com/blacktorn/django-storage-swift',
+    url='https://github.com/dennisv/django-storage-swift',
     author='Dennis Vermeulen',
     author_email='blacktorn@gmail.com',
     license='MIT',
     packages=['swift'],
     install_requires=[
-        'python-swiftclient>=1.4.0',
+        'python-swiftclient>=2.2.0',
         'python-keystoneclient>=0.2.3',
         'six',
         'python-magic>=0.4.10',
     ],
     zip_safe=False,
     classifiers=[
         'Environment :: Web Environment',
         'Framework :: Django',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.3',
+        'Programming Language :: Python :: 3.8',
         'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
         'Topic :: Software Development',
         'Topic :: Software Development :: Libraries :: Application Frameworks',
     ],
 )
```

