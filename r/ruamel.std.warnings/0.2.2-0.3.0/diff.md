# Comparing `tmp/ruamel.std.warnings-0.2.2.tar.gz` & `tmp/ruamel.std.warnings-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ruamel.std.warnings-0.2.2.tar", last modified: Wed Jul 26 12:18:44 2023, max compression
+gzip compressed data, was "ruamel.std.warnings-0.3.0.tar", last modified: Thu Jul 27 19:23:42 2023, max compression
```

## Comparing `ruamel.std.warnings-0.2.2.tar` & `ruamel.std.warnings-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 anthon    (1000) users      (500)        0 2023-07-26 12:18:44.230365 ruamel.std.warnings-0.2.2/
--rw-r--r--   0 anthon    (1000) users      (500)     3813 2023-07-26 12:18:44.230234 ruamel.std.warnings-0.2.2/PKG-INFO
--rw-r--r--   0 anthon    (1000) users      (500)     3201 2023-07-26 12:17:52.000000 ruamel.std.warnings-0.2.2/README.rst
--rw-r--r--   0 anthon    (1000) users      (500)     2016 2023-07-26 12:18:19.000000 ruamel.std.warnings-0.2.2/__init__.py
--rw-r--r--   0 anthon    (1000) users      (500)       97 2023-07-26 12:18:44.000000 ruamel.std.warnings-0.2.2/pyproject.toml
-drwxr-xr-x   0 anthon    (1000) users      (500)        0 2023-07-26 12:18:44.230048 ruamel.std.warnings-0.2.2/ruamel.std.warnings.egg-info/
--rw-r--r--   0 anthon    (1000) users      (500)     3813 2023-07-26 12:18:44.000000 ruamel.std.warnings-0.2.2/ruamel.std.warnings.egg-info/PKG-INFO
--rw-r--r--   0 anthon    (1000) users      (500)      308 2023-07-26 12:18:44.000000 ruamel.std.warnings-0.2.2/ruamel.std.warnings.egg-info/SOURCES.txt
--rw-r--r--   0 anthon    (1000) users      (500)        1 2023-07-26 12:18:44.000000 ruamel.std.warnings-0.2.2/ruamel.std.warnings.egg-info/dependency_links.txt
--rw-r--r--   0 anthon    (1000) users      (500)       61 2023-07-26 12:18:44.000000 ruamel.std.warnings-0.2.2/ruamel.std.warnings.egg-info/entry_points.txt
--rw-r--r--   0 anthon    (1000) users      (500)        1 2023-07-26 12:18:21.000000 ruamel.std.warnings-0.2.2/ruamel.std.warnings.egg-info/not-zip-safe
--rw-r--r--   0 anthon    (1000) users      (500)        7 2023-07-26 12:18:44.000000 ruamel.std.warnings-0.2.2/ruamel.std.warnings.egg-info/top_level.txt
--rw-r--r--   0 anthon    (1000) users      (500)       38 2023-07-26 12:18:44.230403 ruamel.std.warnings-0.2.2/setup.cfg
--rw-rw-r--   0 anthon    (1000) users      (500)    33384 2023-07-26 12:17:52.000000 ruamel.std.warnings-0.2.2/setup.py
+drwxr-xr-x   0 anthon    (1000) users      (500)        0 2023-07-27 19:23:42.624601 ruamel.std.warnings-0.3.0/
+-rw-r--r--   0 anthon    (1000) users      (500)     3813 2023-07-27 19:23:42.624461 ruamel.std.warnings-0.3.0/PKG-INFO
+-rw-r--r--   0 anthon    (1000) users      (500)     3201 2023-07-27 19:22:33.000000 ruamel.std.warnings-0.3.0/README.rst
+-rw-r--r--   0 anthon    (1000) users      (500)     2413 2023-07-27 19:23:13.000000 ruamel.std.warnings-0.3.0/__init__.py
+-rw-r--r--   0 anthon    (1000) users      (500)       97 2023-07-27 19:23:42.000000 ruamel.std.warnings-0.3.0/pyproject.toml
+drwxr-xr-x   0 anthon    (1000) users      (500)        0 2023-07-27 19:23:42.624248 ruamel.std.warnings-0.3.0/ruamel.std.warnings.egg-info/
+-rw-r--r--   0 anthon    (1000) users      (500)     3813 2023-07-27 19:23:42.000000 ruamel.std.warnings-0.3.0/ruamel.std.warnings.egg-info/PKG-INFO
+-rw-r--r--   0 anthon    (1000) users      (500)      308 2023-07-27 19:23:42.000000 ruamel.std.warnings-0.3.0/ruamel.std.warnings.egg-info/SOURCES.txt
+-rw-r--r--   0 anthon    (1000) users      (500)        1 2023-07-27 19:23:42.000000 ruamel.std.warnings-0.3.0/ruamel.std.warnings.egg-info/dependency_links.txt
+-rw-r--r--   0 anthon    (1000) users      (500)       61 2023-07-27 19:23:42.000000 ruamel.std.warnings-0.3.0/ruamel.std.warnings.egg-info/entry_points.txt
+-rw-r--r--   0 anthon    (1000) users      (500)        1 2023-07-27 19:23:16.000000 ruamel.std.warnings-0.3.0/ruamel.std.warnings.egg-info/not-zip-safe
+-rw-r--r--   0 anthon    (1000) users      (500)        7 2023-07-27 19:23:42.000000 ruamel.std.warnings-0.3.0/ruamel.std.warnings.egg-info/top_level.txt
+-rw-r--r--   0 anthon    (1000) users      (500)       38 2023-07-27 19:23:42.624647 ruamel.std.warnings-0.3.0/setup.cfg
+-rw-rw-r--   0 anthon    (1000) users      (500)    33415 2023-07-27 19:22:33.000000 ruamel.std.warnings-0.3.0/setup.py
```

### Comparing `ruamel.std.warnings-0.2.2/PKG-INFO` & `ruamel.std.warnings-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ruamel.std.warnings
-Version: 0.2.2
+Version: 0.3.0
 Summary: extend warnings.warn with callee parameter
 Home-page: https://sourceforge.net/p/ruamel-std-warnings/code/ci/default/tree
 Author: Anthon van der Neut
 Author-email: a.van.der.neut@ruamel.eu
 License: Copyright Ruamel bvba 2007-2023
 Keywords: pypi statistics
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ruamel.std.warnings-0.2.2/README.rst` & `ruamel.std.warnings-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `ruamel.std.warnings-0.2.2/__init__.py` & `ruamel.std.warnings-0.3.0/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # coding: utf-8
 
 from typing import Dict, Any
 
-_package_data: Dict[str, Any] = dict(
+_package_data: Dict[str, Any] = dict(  # NOQA: C408
     full_package_name='ruamel.std.warnings',
-    version_info=(0, 2, 2),
-    __version__='0.2.2',
-    version_timestamp='2023-07-26 14:18:19',
+    version_info=(0, 3, 0),
+    __version__='0.3.0',
+    version_timestamp='2023-07-27 21:23:13',
     author='Anthon van der Neut',
     author_email='a.van.der.neut@ruamel.eu',
     description='extend warnings.warn with callee parameter',
     keywords='pypi statistics',
     entry_points='warning=ruamel.std.warning.__main__:main',
     # entry_points=None,
     license='Copyright Ruamel bvba 2007-2023',
     since=2023,
     # status='α|β|stable',  # the package status on PyPI
     # data_files="",
     # universal=True,  # py2 + py3
     # install_requires=['ruamel.std.pathlib', ],
-    tox=dict(env='3',),  # *->all p->pypy
+    tox=dict(env='3'),  # NOQA: C408  # *->all p->pypy
     python_requires='>=3',
     mypy=False,
 )  # NOQA
 
 
 version_info = _package_data['version_info']
 __version__ = _package_data['__version__']
@@ -36,34 +36,46 @@
 class CalleeWarning(Warning):
     pass
 
 
 class ExtendedWarn:
     warn = org_warnings.warn
 
-    def __call__(self, message, category=None, stacklevel=1, source=None, callee=None):
+    def __call__(
+        self, message, category=None, stacklevel=1, source=None, callee=None,
+    ):
+        # Check if message is already a Warning object
+        if isinstance(message, Warning):
+            category = message.__class__
         if callee:
             assert stacklevel == 1
             if category is not None:
                 filename = callee.__func__.__code__.co_filename
                 lineno = callee.__func__.__code__.co_firstlineno
-                message = CalleeWarning((message, filename, lineno, category))
+                message = ('callee', message, filename, lineno, category)
         else:
             stacklevel += 1
-        self.warn(message, category, stacklevel, source)  # NOQA
+        self.warn(message, category, stacklevel, source)  # NOQA: G010
 
 
-org_warnings.warn = ExtendedWarn()
+org_warnings.warn = warn = ExtendedWarn()
 
 _org_formatwarning = org_warnings.formatwarning
 
 
 def my_formatwarning(message, category, filename, lineno, line):
-    if isinstance(message, CalleeWarning):
-        try:
-            message, filename, lineno, category = message.args[0]
-        except ValueError:  # in case there was no tuple provided
-            pass
+    try:
+        if (
+            not isinstance(message, str)
+            and isinstance(message.args[0], tuple)
+            and len(message.args[0]) == 5
+            and message.args[0][0] == 'callee'
+        ):
+            _, message, filename, lineno, category = message.args[0]
+    except Exception:
+        # show original e.g. when message is not a string,
+        # but has not .args attribute
+        pass
     return _org_formatwarning(message, category, filename, lineno, line)
 
 
 org_warnings.formatwarning = my_formatwarning
```

### Comparing `ruamel.std.warnings-0.2.2/ruamel.std.warnings.egg-info/PKG-INFO` & `ruamel.std.warnings-0.3.0/ruamel.std.warnings.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ruamel.std.warnings
-Version: 0.2.2
+Version: 0.3.0
 Summary: extend warnings.warn with callee parameter
 Home-page: https://sourceforge.net/p/ruamel-std-warnings/code/ci/default/tree
 Author: Anthon van der Neut
 Author-email: a.van.der.neut@ruamel.eu
 License: Copyright Ruamel bvba 2007-2023
 Keywords: pypi statistics
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ruamel.std.warnings-0.2.2/setup.py` & `ruamel.std.warnings-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,17 +45,17 @@
         pass
 
     class NameConstant:
         pass
 
 
 if sys.version_info < (3,):
-    open_kw = dict()
+    open_kw = {}
 else:
-    open_kw = dict(encoding='utf-8')
+    open_kw = dict(encoding='utf-8')  # NOQA: C408
 
 
 if sys.version_info < (2, 7) or platform.python_implementation() == 'Jython':
 
     class Set:
         pass
 
@@ -109,15 +109,15 @@
         elif isinstance(node, Tuple):
             return tuple(map(_convert, node.elts))
         elif isinstance(node, List):
             return list(map(_convert, node.elts))
         elif isinstance(node, Set):
             return set(map(_convert, node.elts))
         elif isinstance(node, Dict):
-            return dict((_convert(k), _convert(v)) for k, v in zip(node.keys, node.values))
+            return {_convert(k): _convert(v) for k, v in zip(node.keys, node.values)}
         elif isinstance(node, NameConstant):
             return node.value
         elif sys.version_info < (3, 4) and isinstance(node, Name):
             if node.id in _safe_names:
                 return _safe_names[node.id]
         elif (
             isinstance(node, UnaryOp)
@@ -140,15 +140,15 @@
             if isinstance(node.op, Add):
                 return left + right
             else:
                 return left - right
         elif isinstance(node, Call):
             func_id = getattr(node.func, 'id', None)
             if func_id == 'dict':
-                return dict((k.arg, _convert(k.value)) for k in node.keywords)
+                return {k.arg: _convert(k.value) for k in node.keywords}
             elif func_id == 'set':
                 return set(_convert(node.args[0]))
             elif func_id == 'date':
                 return datetime.date(*[_convert(k) for k in node.args])
             elif func_id == 'datetime':
                 return datetime.datetime(*[_convert(k) for k in node.args])
         err = SyntaxError('malformed node or string: ' + repr(node))
@@ -198,16 +198,16 @@
                                 print(
                                     '{0:{1}}: {2}'.format(index, w, line).encode('utf-8'),
                                     end="",
                                 )
                                 if index == e.lineno - 1:
                                     print(
                                         '{0:{1}}  {2}^--- {3}'.format(
-                                            ' ', w, ' ' * e.offset, e.node
-                                        )
+                                            ' ', w, ' ' * e.offset, e.node,
+                                        ),
                                     )
                         raise
                     break
                 lines.append(line)
             else:
                 raise NotImplementedError
     return data
@@ -396,15 +396,15 @@
             res.append('.' + d)
         return res
 
     @property
     def package_dir(self):
         d = {
             # don't specify empty dir, clashes with package_data spec
-            self.full_package_name: '.'
+            self.full_package_name: '.',
         }
         if 'extra_packages' in self._pkg_data:
             return d
         # if len(self.split) > 1:  # only if package namespace
         #     d[self.split[0]] = self.namespace_directories(1)[0]
         # print('d', d, os.getcwd())
         return d
@@ -434,15 +434,15 @@
             return
 
         # if hgi and hgi.base are both in namespace_packages matching
         # against the top (hgi.) it suffices to find minus-e and non-minus-e
         # installed packages. As we don't know the order in namespace_packages
         # do some magic
         prefix = self.split[0]
-        prefixes = set([prefix, prefix.replace('_', '-')])
+        prefixes = {prefix, prefix.replace('_', '-')}
         for p in sys.path:
             if not p:
                 continue  # directory with setup.py
             if os.path.exists(os.path.join(p, 'setup.py')):
                 continue  # some linked in stuff might not be hgi based
             if not os.path.isdir(p):
                 continue
@@ -457,27 +457,27 @@
                 full_name = os.path.join(p, fn)
                 # not in prefixes the toplevel is never changed from _ to -
                 if fn == prefix and os.path.isdir(full_name):
                     # directory -> other, non-minus-e, install
                     if self.command == 'develop':
                         raise InstallationError(
                             'Cannot mix develop (pip install -e),\nwith '
-                            'non-develop installs for package name {0}'.format(fn)
+                            'non-develop installs for package name {0}'.format(fn),
                         )
                 elif fn == prefix:
                     raise InstallationError('non directory package {0} in {1}'.format(fn, p))
                 for pre in [x + '.' for x in prefixes]:
                     if fn.startswith(pre):
                         break
                 else:
                     continue  # hgiabc instead of hgi.
                 if fn.endswith('-link') and self.command == 'install':
                     raise InstallationError(
                         'Cannot mix non-develop with develop\n(pip install -e)'
-                        ' installs for package name {0}'.format(fn)
+                        ' installs for package name {0}'.format(fn),
                     )
 
     def entry_points(self, script_name=None, package_name=None):
         """normally called without explicit script_name and package name
         the default console_scripts entry depends on the existence of __main__.py:
         if that file exists then the function main() in there is used, otherwise
         the in __init__.py.
@@ -487,15 +487,15 @@
         scriptname is the last part of the full package path (split on '.')
         if the ep entry is a simple string without "=", that is assumed to be
         the name of the script.
         """
 
         def pckg_entry_point(name):
             return '{0}{1}:main'.format(
-                name, '.__main__' if os.path.exists('__main__.py') else ""
+                name, '.__main__' if os.path.exists('__main__.py') else "",
             )
 
         ep = self._pkg_data.get('entry_points', True)
         if isinstance(ep, dict):
             return ep
         if ep is None:
             return None
@@ -508,16 +508,16 @@
             script_name = ep
         if package_name is None:
             package_name = self.full_package_name
         if not script_name:
             script_name = package_name.rsplit('.', 1)[-1]
         return {
             'console_scripts': [
-                '{0} = {1}'.format(script_name, pckg_entry_point(package_name))
-            ]
+                '{0} = {1}'.format(script_name, pckg_entry_point(package_name)),
+            ],
         }
 
     @property
     def url(self):
         url = self._pkg_data.get('url')
         if url:
             return url
@@ -582,16 +582,16 @@
                     'Intended Audience :: Developers',
                     'License :: '
                     + ('OSI Approved :: MIT' if self.has_mit_lic() else 'Other/Proprietary')
                     + ' License',
                     'Operating System :: OS Independent',
                     'Programming Language :: Python',
                 ]
-                + [self.pn(x) for x in self._pkg_data.get('classifiers', [])]
-            )
+                + [self.pn(x) for x in self._pkg_data.get('classifiers', [])],
+            ),
         )
 
     @property
     def keywords(self):
         return self.pn(self._pkg_data.get('keywords', []))
 
     @property
@@ -839,20 +839,20 @@
         print('pip:       ', pip.__version__)
         print('setuptools:', setuptools.__version__)
         print('wheel:     ', wheel.__version__)
     nsp = NameSpacePackager(pkg_data)
     nsp.check()
     # nsp.create_dirs()
     MySdist.nsp = nsp
-    cmdclass = dict(install_lib=MyInstallLib, sdist=MySdist)
+    cmdclass = dict(install_lib=MyInstallLib, sdist=MySdist)  # NOQA: C408
     if _bdist_wheel_available:
         MyBdistWheel.nsp = nsp
         cmdclass['bdist_wheel'] = MyBdistWheel
 
-    kw = dict(
+    kw = dict(  # NOQA: C408
         name=nsp.full_package_name,
         version=version_str,
         packages=nsp.packages,
         python_requires=nsp.python_requires,
         url=nsp.url,
         author=nsp.author,
         author_email=nsp.author_email,
```

