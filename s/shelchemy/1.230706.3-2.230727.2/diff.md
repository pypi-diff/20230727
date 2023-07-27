# Comparing `tmp/shelchemy-1.230706.3.tar.gz` & `tmp/shelchemy-2.230727.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shelchemy-1.230706.3.tar", max compression
+gzip compressed data, was "shelchemy-2.230727.2.tar", max compression
```

## Comparing `shelchemy-1.230706.3.tar` & `shelchemy-2.230727.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35149 2022-08-23 03:49:07.000000 shelchemy-1.230706.3/LICENSE
--rw-r--r--   0        0        0     1410 2023-07-20 20:06:07.115439 shelchemy-1.230706.3/README.md
--rw-r--r--   0        0        0     1036 2023-07-20 20:06:09.495440 shelchemy-1.230706.3/pyproject.toml
--rw-r--r--   0        0        0      501 2023-07-06 23:38:55.083313 shelchemy-1.230706.3/src/shelchemy/__init__.py
--rw-r--r--   0        0        0     8626 2023-07-20 20:05:10.823409 shelchemy-1.230706.3/src/shelchemy/cache.py
--rw-r--r--   0        0        0     1758 2022-09-06 20:21:46.000000 shelchemy-1.230706.3/src/shelchemy/lazy.py
--rw-r--r--   0        0        0     5398 2023-07-20 20:06:04.347437 shelchemy-1.230706.3/src/shelchemy/locker.py
--rw-r--r--   0        0        0     2097 2023-01-12 19:31:50.000000 shelchemy-1.230706.3/src/shelchemy/scheduler.py
--rw-r--r--   0        0        0      333 2023-07-06 23:38:55.087313 shelchemy-1.230706.3/src/shelchemy/sqla.py
--rw-r--r--   0        0        0     2128 1970-01-01 00:00:00.000000 shelchemy-1.230706.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-08-23 03:49:07.000000 shelchemy-2.230727.2/LICENSE
+-rw-r--r--   0        0        0     3109 2023-07-27 18:35:15.115736 shelchemy-2.230727.2/README.md
+-rw-r--r--   0        0        0     1036 2023-07-27 18:35:17.363737 shelchemy-2.230727.2/pyproject.toml
+-rw-r--r--   0        0        0      501 2023-07-06 23:38:55.083313 shelchemy-2.230727.2/src/shelchemy/__init__.py
+-rw-r--r--   0        0        0     9004 2023-07-27 18:35:09.087734 shelchemy-2.230727.2/src/shelchemy/cache.py
+-rw-r--r--   0        0        0     2106 2023-07-27 18:04:10.858817 shelchemy-2.230727.2/src/shelchemy/lazy.py
+-rw-r--r--   0        0        0     7102 2023-07-27 18:04:10.878817 shelchemy-2.230727.2/src/shelchemy/locker.py
+-rw-r--r--   0        0        0     2102 2023-07-27 16:15:38.255517 shelchemy-2.230727.2/src/shelchemy/scheduler.py
+-rw-r--r--   0        0        0      333 2023-07-06 23:38:55.087313 shelchemy-2.230727.2/src/shelchemy/sqla.py
+-rw-r--r--   0        0        0     3827 1970-01-01 00:00:00.000000 shelchemy-2.230727.2/PKG-INFO
```

### Comparing `shelchemy-1.230706.3/LICENSE` & `shelchemy-2.230727.2/LICENSE`

 * *Files identical despite different names*

### Comparing `shelchemy-1.230706.3/pyproject.toml` & `shelchemy-2.230727.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shelchemy"
-version = "1.230706.3"
+version = "2.230727.2"
 description = "Shelve-like dict using sqlalchemy as a backend, and lazy scheduler for resuming tasks"
 authors = ["davips <dpsabc@gmail.com>"]
 license = "GPL"
 readme = 'README.md'
 packages = [
     { include = "shelchemy", from = "src" }
 ]
```

### Comparing `shelchemy-1.230706.3/src/shelchemy/cache.py` & `shelchemy-2.230727.2/src/shelchemy/cache.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,24 +31,22 @@
 from shelchemy import memory
 from shelchemy.sqla import Base, Content
 
 VT = TypeVar("VT")
 
 
 def check(key):
-    if not isinstance(key, str):
-        try:
-            dump = dumps(key, protocol=5)
-        except Exception as e:
-            print(e)
-            raise WrongKeyType(f"Key must be string or serializable (pickable), not {type(key)}.", key)
-        key = md5(dump).hexdigest()
-    elif len(key) not in [32, 40]:
-        key = md5(key.encode()).hexdigest()
-    return key
+    if isinstance(key, str):
+        return key
+    try:
+        dump = dumps(key, protocol=5)
+    except Exception as e:  # pragma: no cover
+        print(e)
+        raise WrongKeyType(f"Key must be string or serializable (pickable), not {type(key)}.", key)
+    return md5(dump).hexdigest()
 
 
 class Cache:
     r"""
     Dict-like persistence based on SQLAlchemy
 
     string or serializable (pickle) keys only
@@ -56,75 +54,98 @@
     When len(key) not in [32, 40], key is internally hashed to a MD5 hexdigest
 
     Usage:
 
     >>> from shelchemy import sopen
     >>> d = Cache("sqlite+pysqlite:////tmp/sqla-test.db")
     >>> d["x"] = 5
-    >>> d["x"]
-    5
+    >>> d["b"] = None
+    >>> d["x"], d["b"]
+    (5, None)
+    >>> try:
+    ...     d["xxx"]
+    ... except KeyError as m:
+    ...     print(m)
+    'xxx'
     >>> for k, v in d.items():
     ...     print(k, v)
-    9dd4e461268c8034f5c8564e155c67a6 5
+    x 5
+    b None
     >>> "x" in d
     True
     >>> len(d)
-    1
+    2
     >>> del d["x"]
     >>> "x" in d
     False
     >>> d
-    {}
+    {'b': None}
     >>> with sopen() as db:
     ...     "x" in db
     ...     db
     ...     db["x"] = b"asd"
     ...     db
-    ...     db["9dd4e461268c8034f5c8564e155c67a6"] == b"asd"
+    ...     db["x"] == b"asd"
     ...     "x" in db
     ...     db.x == b"asd"
     ...     del db["x"]
     ...     "x" in db
     False
     {}
-    {'9dd4e461268c8034f5c8564e155c67a6': b'asd'}
+    {'x': b'asd'}
     True
     True
     True
     False
+    >>> d.update({"a": b"by"})
+    >>> d.a
+    b'by'
+    >>> list(d.keys())
+    ['b', 'a']
+    >>> d
+    {'b': None, 'a': b'by'}
+    >>> str(d)
+    "{'b': None, 'a': b'by'}"
+    >>> d = Cache("sqlite+pysqlite:////tmp/sqla-test.db", autopack=False)
+    >>> d[[1,2,"a"]] = b"only bytes when autopack=False"
+    >>> d[[1,2,"a"]]
+    b'only bytes when autopack=False'
+    >>> d.update({"a": b"by"})
+    >>> d.a
+    b'by'
     """
 
     def __init__(
         self, session=memory, ondup="overwrite", autopack=True, safepack=False, stablepack=False, debug=False, _engine=None
     ):
         if isinstance(session, str):
 
             @contextmanager
             def sessionctx():
                 engine = create_engine(url=session, echo=debug)
                 self._engine = engine
                 session_ = Session(engine, autoflush=False)
                 try:
                     yield session_
-                except:
+                except:  # pragma: no cover
                     session_.rollback()
                     raise
                 finally:
                     session_.close()
 
         else:
-            if _engine is None:
+            if _engine is None:  # pragma: no cover
                 raise Exception(f"Missing `_engine` for external non string session.")
             self._engine = _engine
 
             @contextmanager
             def sessionctx():
                 try:
                     yield session
-                except:
+                except:  # pragma: no cover
                     session.rollback()
                     raise
                 finally:
                     session.close()
 
         self.sessionctx = sessionctx
         self.ondup = ondup
@@ -135,15 +156,15 @@
     def ensure_build(self, query__f):
         with self.sessionctx() as session:
             try:
                 return query__f(session)
             except Exception as e:
                 try:
                     Base.metadata.create_all(self._engine)
-                except:
+                except:  # pragma: no cover
                     raise e from None
         return query__f(session)
 
     def __contains__(self, key):
         key = check(key)
         return self.ensure_build(lambda session: session.query(Content).filter_by(id=key).first() is not None)
 
@@ -151,21 +172,19 @@
         return self.ensure_build(lambda session: (c.id for c in session.query(Content).all()))
 
     def __setitem__(self, key: str, value, packing=True):
         key = check(key)
         if self.autopack and packing:
             try:
                 from safeserializer.compression import pack
-            except ModuleNotFoundError:
+            except ModuleNotFoundError:  # pragma: no cover
                 raise Exception(
                     "You need to install optional packages `safeserializer` and `lz4` to be able to use compression inside shelchemy."
                 )
             value = pack(value, ensure_determinism=self.stablepack, unsafe_fallback=not self.safepack)
-        elif isinstance(value, str):
-            value = value.encode()
 
         def f(session):
             if self.ondup == "overwrite":
                 session.query(Content).filter_by(id=key).delete()
             if self.ondup == "stop" or session.query(Content).filter_by(id=key).first() is None:
                 content = Content(id=key, blob=value)
                 session.add(content)
@@ -176,46 +195,45 @@
     def update(self, dic, packing=True):
         def f(session):
             for k, v in dic.items():
                 k = check(k)
                 if self.autopack and packing:
                     try:
                         from safeserializer.compression import pack
-                    except ModuleNotFoundError:
+                    except ModuleNotFoundError:  # pragma: no cover
                         raise Exception(
                             "You need to install optional packages `safeserializer` and `lz4` to be able to use compression inside shelchemy."
                         )
                     v = pack(v, ensure_determinism=self.stablepack, unsafe_fallback=not self.safepack)
-                elif isinstance(v, str):
-                    v = v.encode()
 
                 if self.ondup == "overwrite":
                     session.query(Content).filter_by(id=k).delete()
                 if self.ondup == "stop" or session.query(Content).filter_by(id=k).first() is None:
                     content = Content(id=k, blob=v)
                     session.add(content)
             session.commit()
 
         self.ensure_build(f)
 
     def __getitem__(self, key, packing=True):
         key = check(key)
 
         def f(session):
-            if ret := session.query(Content).get(key):
-                if ret is not None:
-                    ret = ret.blob
-                    if self.autopack and packing:
-                        try:
-                            from safeserializer.compression import unpack
-                        except ModuleNotFoundError:
-                            raise Exception(
-                                "You need to install optional packages `safeserializer` and `lz4` to be able to use compression inside shelchemy."
-                            )
-                        ret = unpack(ret)
+            ret = session.query(Content).get(key)
+            if ret is None:
+                raise KeyError(key)
+            ret = ret.blob
+            if self.autopack and packing:
+                try:
+                    from safeserializer.compression import unpack
+                except ModuleNotFoundError:  # pragma: no cover
+                    raise Exception(
+                        "You need to install optional packages `safeserializer` and `lz4` to be able to use compression inside shelchemy."
+                    )
+                ret = unpack(ret)
             return ret
 
         return self.ensure_build(f)
 
     def __delitem__(self, key):
         key = check(key)
 
@@ -225,15 +243,15 @@
 
         self.ensure_build(f)
 
     def __getattr__(self, key):
         key_ = check(key)
         if key_ in self:
             return self[key_]
-        return self.__getattribute__(key)
+        return self.__getattribute__(key)  # pragma: no cover
 
     def __len__(self):
         return self.ensure_build(lambda session: session.query(Content).count())
 
     def __repr__(self):
         return repr(self.asdict)
 
@@ -241,15 +259,15 @@
         return repr(self)
 
     @property
     def asdict(self):
         return {k: self[k] for k in self}
 
     def copy(self):
-        raise NotImplementedError
+        raise NotImplementedError  # pragma: no cover
 
     def keys(self):
         return iter(self)
 
     def items(self):
         for k in self.keys():
             yield k, self[k]
```

### Comparing `shelchemy-1.230706.3/src/shelchemy/lazy.py` & `shelchemy-2.230727.2/src/shelchemy/lazy.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,14 +19,36 @@
 #  works or verbatim, obfuscated, compiled or rewritten versions of any
 #  part of this work is illegal and it is unethical regarding the effort and
 #  time spent here.
 #
 
 
 def ichunks(items, binsize, asgenerators=True):
+    """
+    >>> for ch in ichunks([1,2,3,4,5], 2):
+    ...     print(list(ch))
+    [1, 2]
+    [3, 4]
+    [5]
+    >>> for ch in ichunks([1,2,3,4,5], 2, asgenerators=False):
+    ...     print(ch)
+    [1, 2]
+    [3, 4]
+    [5]
+
+    Parameters
+    ----------
+    items
+    binsize
+    asgenerators
+
+    Returns
+    -------
+
+    """
     consumed = [0]
     sent = [0]
     it = iter(items)
 
     def g():
         c = 0
         while c < binsize:
@@ -41,9 +63,9 @@
             c += 1
 
     while True:
         yield g() if asgenerators else list(g())
         if consumed[0] is None:
             return
         sent[0] += binsize
-        if consumed[0] < sent[0]:
+        if consumed[0] < sent[0]:  # pragma: no cover
             raise Exception("Cannot traverse a chunk before the previous one is consumed.", consumed[0], sent[0])
```

### Comparing `shelchemy-1.230706.3/src/shelchemy/scheduler.py` & `shelchemy-2.230727.2/src/shelchemy/scheduler.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,31 +20,31 @@
     >>> names2 = ["c"]
     >>> names3 = ["d","e"]
     >>> storage = {}
     >>> for name in Scheduler(storage, timeout=10) << names1 << names2 << names3:
     ...    print(f"Processing {name}")
     ...    sleep(0.1)
     ...    print(f"{name} processed!")
-    'a' is new, started
+    'a' is new, starting
     Processing a
     a processed!
     'a' done
-    'b' is new, started
+    'b' is new, starting
     Processing b
     b processed!
     'b' done
-    'c' is new, started
+    'c' is new, starting
     Processing c
     c processed!
     'c' done
-    'd' is new, started
+    'd' is new, starting
     Processing d
     d processed!
     'd' done
-    'e' is new, started
+    'e' is new, starting
     Processing e
     e processed!
     'e' done
     >>> storage
     {'a': b'd', 'b': b'd', 'c': b'd', 'd': b'd', 'e': b'd'}
     >>> for name in Scheduler(storage, timeout=10) << names1 << names2 << names3:
     ...    print(f"Processing {name}")
```

