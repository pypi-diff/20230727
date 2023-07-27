# Comparing `tmp/kioss-0.0.9.tar.gz` & `tmp/kioss-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kioss-0.0.9.tar", last modified: Wed Jul 26 07:24:13 2023, max compression
+gzip compressed data, was "kioss-0.1.0.tar", last modified: Thu Jul 27 15:38:02 2023, max compression
```

## Comparing `kioss-0.0.9.tar` & `kioss-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:24:13.961039 kioss-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-26 07:23:58.000000 kioss-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-26 07:24:13.961039 kioss-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-26 07:23:58.000000 kioss-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:24:13.957039 kioss-0.0.9/kioss/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-26 07:23:58.000000 kioss-0.0.9/kioss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12632 2023-07-26 07:23:58.000000 kioss-0.0.9/kioss/pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-26 07:23:58.000000 kioss-0.0.9/kioss/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:24:13.957039 kioss-0.0.9/kioss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-26 07:24:13.000000 kioss-0.0.9/kioss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-26 07:24:13.000000 kioss-0.0.9/kioss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 07:24:13.000000 kioss-0.0.9/kioss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-26 07:24:13.000000 kioss-0.0.9/kioss.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 07:24:13.961039 kioss-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-26 07:23:58.000000 kioss-0.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:24:13.961039 kioss-0.0.9/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-07-26 07:23:58.000000 kioss-0.0.9/test/test_pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-26 07:23:58.000000 kioss-0.0.9/test/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:38:02.883457 kioss-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-27 15:37:54.000000 kioss-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-27 15:38:02.879457 kioss-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-07-27 15:37:54.000000 kioss-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:38:02.879457 kioss-0.1.0/kioss/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 15:37:54.000000 kioss-0.1.0/kioss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15088 2023-07-27 15:37:54.000000 kioss-0.1.0/kioss/pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-27 15:37:54.000000 kioss-0.1.0/kioss/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:38:02.879457 kioss-0.1.0/kioss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-27 15:38:02.000000 kioss-0.1.0/kioss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-27 15:38:02.000000 kioss-0.1.0/kioss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 15:38:02.000000 kioss-0.1.0/kioss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-27 15:38:02.000000 kioss-0.1.0/kioss.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 15:38:02.883457 kioss-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-27 15:37:54.000000 kioss-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:38:02.879457 kioss-0.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     8574 2023-07-27 15:37:54.000000 kioss-0.1.0/test/test_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-27 15:37:54.000000 kioss-0.1.0/test/test_util.py
```

### Comparing `kioss-0.0.9/LICENSE` & `kioss-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kioss-0.0.9/kioss/pipe.py` & `kioss-0.1.0/kioss/pipe.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+import atexit
 import itertools
 import logging
 import time
 import timeit
 from concurrent.futures import ThreadPoolExecutor
 from datetime import datetime
 from functools import reduce
 from queue import Empty, Queue
-from typing import Callable, Iterable, Iterator, List, TypeVar, Union
+from typing import Callable, Iterable, Iterator, List, Tuple, Type, TypeVar, Union
 
 import kioss.util as util
 
 T = TypeVar("T")
 R = TypeVar("R")
 
 
@@ -21,75 +22,71 @@
     Args:
         source (Union[Iterable[T], Iterator[T]]): The iterator or iterable containing elements for the pipeline.
 
     Attributes:
         iterator (Iterator[T]): The iterator containing elements for the pipeline.
     """
 
-    def __init__(self, source: Union[Iterable[T], Iterator[T]]) -> None:
+    def __init__(self, source: Union[Iterable[T], Iterator[T]] = []) -> None:
         self.iterator: Iterator[T] = iter(source)
 
     def __next__(self) -> T:
         return next(self.iterator)
 
     def __iter__(self) -> T:
         return self
 
-    def chain(self, *others: Iterable["Pipe[T]"]) -> "Pipe[T]":
+    def __add__(self, other: "Pipe[T]") -> "Pipe[T]":
+        return self.chain(other)
+
+    def chain(self, *others: Tuple["Pipe[T]"]) -> "Pipe[T]":
         """
-        Create a new Pipe by chaining the elements of this Pipe with the elements from other Pipes.
+        Create a new Pipe by chaining the elements of this Pipe with the elements from other Pipes. The elements of a given Pipe are yielded after its predecessor Pipe is exhausted.
 
         Args:
-            *others (Iterable[Pipe[T]]): One or more additional Pipe instances to chain with this Pipe.
+            *others ([Pipe[T]]): One or more additional Pipe instances to chain with this Pipe.
 
         Returns:
             Pipe[T]: A new Pipe instance with elements from this Pipe followed by elements from other Pipes.
         """
         return Pipe[T](itertools.chain(self, *others))
 
-    def merge(self, *others: Iterable["Pipe[T]"]) -> "Pipe[T]":
+    def mix(self, *others: "Pipe[T]") -> "Pipe[T]":
         """
-        Merge this Pipe with other Pipes, returning a new Pipe with elements from all Pipes in their order of occurrence.
+        Mix this Pipe with other Pipes using one thread per pipe, returning a new Pipe instance concurrently yielding elements from self and others in any order.
 
         Args:
-            *others (Iterable[Pipe[T]]): One or more additional Pipe instances to merge with this Pipe.
+            *others ([Pipe[T]]): One or more additional Pipe instances to mix with this Pipe.
 
         Returns:
-            Pipe[T]: A new Pipe instance with elements from this Pipe followed by elements from other Pipes.
+            Pipe[T]: A new Pipe instance concurrently yielding elements from self and others in any order.
         """
-        return _ConcurrentlyMergingPipe[T]([self, *others])
+        return _RasingPipe[R](_ConcurrentlyMergingPipe[T]([self, *others]))
 
     def map(
-        self, func: Callable[[T], R], num_threads: int = 0, sidify: bool = False
+        self, func: Callable[[T], R], n_threads: int = 0, sidify: bool = False
     ) -> "Pipe[R]":
         """
         Apply a function to each element of the Pipe, creating a new Pipe with the mapped elements.
 
         Args:
             func (Callable[[T], R]): The function to be applied to each element.
-            num_threads (int, optional): The number of threads for concurrent mapping (default is 0, meaning single-threaded).
+            n_threads (int, optional): The number of threads for concurrent mapping (default is 0, meaning single-threaded).
             sidify (bool, optional): If True, apply function with side effect wrapping (default is False).
 
         Returns:
             Pipe[R]: A new Pipe instance with elements resulting from applying the function to each element.
         """
         if sidify:
             func = util.sidify(func)
 
-        if num_threads <= 1:
+        if n_threads <= 0:
             return Pipe[R](map(func, self))
         else:
-
-            def iterable():
-                executor = ThreadPoolExecutor(max_workers=num_threads)
-                # non consumed map results block the worker that produced them, hence it makes it compatible with self.slow()
-                yield from executor.map(func, self)
-                executor.shutdown()
-
-            return Pipe[R](iter(iterable()))
+            return _RasingPipe[R](_ConcurrentlyMappingPipe[R](func, self, n_threads))
 
     def flatten(self: "Pipe[Iterator[R]]") -> "Pipe[R]":
         """
         Flatten the elements of the Pipe, which are assumed to be iterators, creating a new Pipe with individual elements.
 
         Returns:
             Pipe[R]: A new Pipe instance with individual elements obtained by flattening the original elements.
@@ -119,68 +116,72 @@
             max_window_seconds (float, optional): The maximum time window for batching elements (default is infinity).
 
         Returns:
             Pipe[List[T]]: A new Pipe instance with lists containing batches of elements.
         """
         return _BatchingPipe[T](self, max_size, time_window_seconds)
 
-    def slow(self, freq: int) -> "Pipe[T]":
+    def slow(self, freq: float) -> "Pipe[T]":
         """
         Slow down the iteration of elements in the Pipe, creating a new Pipe with a specified frequency.
 
         Args:
-            freq (int): The frequency (in milliseconds) at which elements are iterated.
+            freq (float): The frequency (in milliseconds) at which elements are iterated.
 
         Returns:
             Pipe[T]: A new Pipe instance with elements iterated at the specified frequency.
         """
         return Pipe[T](_SlowingIterator(self, freq))
 
-    def head(self, n) -> "Pipe[T]":
+    def head(self, n: int) -> "Pipe[T]":
         """
         Limit the number of elements in the Pipe, creating a new Pipe with the first `n` elements.
 
         Args:
-            n: The number of elements to include in the new Pipe.
+            n (int): The number of elements to include in the new Pipe.
 
         Returns:
             Pipe[T]: A new Pipe instance with the first `n` elements.
         """
         return Pipe[T](itertools.islice(self, n))
 
-    def catch(self) -> "Pipe[T]":
+    def catch(self, *classes: Type[Exception], ignore=False) -> "Pipe[T]":
         """
-        Catch any errors that occur during the iteration of elements in the Pipe.
+        Any error whose class is exception_class or a subclass of it will be catched and yielded.
+
+        Args:
+            exception_class (Type[Exception]): The class of exceptions to catch
+            ingore (bool): If True then the encountered exception_class errors will be skipped.
 
         Returns:
             Pipe[T]: A new Pipe instance with error handling capability.
         """
-        return _CatchingPipe[T](self)
+        return _CatchingPipe[T](self, classes, ignore)
 
-    def log(self) -> "Pipe[T]":
+    def log(self, objects_description: str = "elements") -> "Pipe[T]":
         """
         Log the elements of the Pipe as they are iterated.
 
         Returns:
             Pipe[T]: A new Pipe instance with logging capability.
         """
-        return _LoggingPipe[T](self)
+        return _LoggingPipe[T](self, objects_description)
 
-    def reduce(self, f: Callable[[R, T], R], initial: R) -> R:
+    def reduce(self, func: Callable[[R, T], R], initial: R) -> R:
         """
         Reduce the elements of the Pipe using a binary function, starting from the given initial value.
 
         Args:
-            f (Callable[[R, T], R]): The binary function used for reduction.
+            func (Callable[[R, T], R]): The binary function used for reduction.
             initial (R): The initial value for the reduction.
 
         Returns:
             R: The result of the reduction.
         """
-        return reduce(f, self, initial)
+        return reduce(func, self, initial)
 
     def collect(self, limit: int = float("inf")) -> List[T]:
         """
         Convert the elements of the Pipe into a list. The entire pipe will be iterated, even after reaching the optional limit.
 
         Args:
             limit (int, optional): The maximum number of elements to include in the list (default is infinity).
@@ -200,29 +201,29 @@
 
         def iterate():
             for _ in self:
                 pass
 
         return timeit.timeit(iterate, number=1)
 
-    def superintend(self, num_error_samples: int = 8) -> None:
+    def superintend(self, n_error_samples: int = 8) -> None:
         """
         Superintend the Pipe: iterate over the pipe until it is exhausted and raise a RuntimeError if any exceptions occur during iteration.
 
         Args:
-            num_error_samples (int, optional): The maximum number of error samples to include in the RuntimeError message (default is 8).
+            n_error_samples (int, optional): The maximum number of error samples to include in the RuntimeError message (default is 8).
         Raises:
             RuntimeError: If any exception is catched during iteration.
         """
         if errors := (
-            self.catch()
+            self.catch(Exception, ignore=False)
             .log()
             .filter(lambda elem: isinstance(elem, Exception))
             .map(repr)
-            .collect(limit=num_error_samples)
+            .collect(limit=n_error_samples)
         ):
             raise RuntimeError(errors)
 
 
 class _FlatteningPipe(Pipe[R]):
     def __init__(self, iterator: Iterator[Iterator[R]]) -> None:
         super().__init__(iterator)
@@ -233,37 +234,48 @@
             return next(self.current_iterator_elem)
         except StopIteration:
             self.current_iterator_elem = iter(super().__next__())
             return next(self)
 
 
 class _CatchingPipe(Pipe[T]):
+    def __init__(
+        self, iterator: Iterator[T], classes: Tuple[Type[Exception]], ignore: bool
+    ) -> None:
+        super().__init__(iterator)
+        self.classes = classes
+        self.ignore = ignore
+
     def __next__(self) -> T:
         try:
             return super().__next__()
-        except Exception as e:
-            if isinstance(e, StopIteration):
-                raise
+        except StopIteration:
+            raise
+        except self.classes as e:
+            if self.ignore:
+                return next(self)
             else:
                 return e
 
 
 class _LoggingPipe(Pipe[T]):
-    def __init__(self, iterator: Iterator[T]) -> None:
+    def __init__(self, iterator: Iterator[T], objects_description: str) -> None:
         super().__init__(iterator)
         logging.getLogger().setLevel(logging.INFO)
+        self.objects_description = objects_description
         self.yields_count = 0
         self.errors_count = 0
         self.last_log_at_yields_count = 0
         self.start_time = time.time()
 
     def _log(self) -> None:
         logging.info(
-            "%s elements have been yielded in elapsed time '%s', with %s errors produced.",
+            "%s `%s` have been yielded in elapsed time '%s', with %s errors produced.",
             self.yields_count,
+            self.objects_description,
             str(
                 datetime.fromtimestamp(time.time())
                 - datetime.fromtimestamp(self.start_time)
             ),
             self.errors_count,
         )
 
@@ -282,94 +294,148 @@
             self._log()
             self.last_log_at_yields_count = self.yields_count + self.errors_count
 
         return elem
 
 
 class _SlowingIterator(Pipe[T]):
-    def __init__(self, iterator: Iterator[T], freq: int) -> None:
+    def __init__(self, iterator: Iterator[T], freq: float) -> None:
         super().__init__(iterator)
         self.freq = freq
         self.start = None
         self.yields_count = 0
 
     def __next__(self) -> T:
         if not self.start:
             self.start = time.time()
         while True:
+            next_elem = super().__next__()
             while self.yields_count > (time.time() - self.start) * self.freq:
-                time.sleep(1 / self.freq)
+                time.sleep(0.001)
             self.yields_count += 1
-            return super().__next__()
+            return next_elem
 
 
 class _BatchingPipe(Pipe[List[T]]):
     def __init__(
         self, iterator: Iterator[T], max_size: int, max_window_seconds: float
     ) -> None:
         super().__init__(iterator)
         self.max_size = max_size
         self.max_window_seconds = max_window_seconds
 
     def __next__(self) -> List[T]:
         start_time = time.time()
-        batch = [next(self.iterator)]
+        batch = [super().__next__()]
         try:
             while (
                 len(batch) < self.max_size
                 and (time.time() - start_time) < self.max_window_seconds
             ):
-                batch.append(next(self.iterator))
+                batch.append(super().__next__())
             return batch
         except StopIteration:
             if batch:
                 return batch
             else:
                 raise
 
 
 class _ConcurrentlyMergingPipe(Pipe[T]):
-    MIN_SLEEP_TIME_MS = 0.005
     MAX_NUM_WAITING_ELEMS_PER_THREAD = 16
 
     def __init__(self, iterators: List[Iterator[T]]) -> None:
         super().__init__(
-            iter(
-                _ConcurrentlyMergingPipe._concurrently_merging_iterable(
-                    iterators,
-                    max_queue_size=_ConcurrentlyMergingPipe.MAX_NUM_WAITING_ELEMS_PER_THREAD
-                    * len(iterators),
-                )
+            self._concurrently_merging_iterable(
+                iterators,
+                Queue(self.MAX_NUM_WAITING_ELEMS_PER_THREAD * len(iterators)),
             )
         )
 
     @staticmethod
-    def _pull_in_queue(
-        iterator: Iterator[T], queue: Queue, max_queue_size: int
-    ) -> None:
-        for elem in iterator:
-            backoffed_sleep_time = _ConcurrentlyMergingPipe.MIN_SLEEP_TIME_MS
-            while queue.qsize() > max_queue_size:
-                time.sleep(backoffed_sleep_time)
-                backoffed_sleep_time *= 2
-            queue.put(elem)
-
-    @staticmethod
     def _concurrently_merging_iterable(
-        iterators: List[Iterator[T]], max_queue_size: int
+        iterators: List[Iterator[T]], queue: Queue[T]
     ) -> Iterator[T]:
-        queue = Queue()
         with ThreadPoolExecutor(max_workers=len(iterators)) as executor:
-            futures = [
-                executor.submit(
-                    _ConcurrentlyMergingPipe._pull_in_queue,
+
+            def pull_job(iterator: Iterator[T]):
+                while True:
+                    try:
+                        queue.put(next(iterator))
+                    except StopIteration:
+                        break
+                    except Exception as e:
+                        queue.put(_CatchedError(e))
+
+            futures = [executor.submit(pull_job, iterator) for iterator in iterators]
+            while not queue.empty() or not all((future.done() for future in futures)):
+                try:
+                    yield queue.get(timeout=0.01)
+                except Empty:
+                    pass
+
+
+class _ConcurrentlyMappingPipe(Pipe[R]):
+    MAX_NUM_WAITING_ELEMS_PER_THREAD = 16
+
+    def __init__(
+        self, func: Callable[[T], R], iterator: Iterator[T], n_threads: int
+    ) -> None:
+        super().__init__(
+            iter(
+                self._concurrently_mapping_iterable(
+                    func,
                     iterator,
-                    queue,
-                    max_queue_size,
+                    n_threads=n_threads,
+                    max_queue_size=self.MAX_NUM_WAITING_ELEMS_PER_THREAD * n_threads,
                 )
-                for iterator in iterators
-            ]
-            while not queue.empty() or not all((future.done() for future in futures)):
+            )
+        )
+
+    @staticmethod
+    def _concurrently_mapping_iterable(
+        func: Callable[[T], R], iterator: Iterator[T], n_threads, max_queue_size: int
+    ) -> Iterator[T]:
+        input_queue: Queue[T] = Queue(maxsize=max_queue_size)
+        output_queue: Queue[R] = Queue(maxsize=max_queue_size)
+
+        with ThreadPoolExecutor(max_workers=n_threads + 1) as executor:
+            input_feeder_future = executor.submit(
+                lambda: util.iterate(map(input_queue.put, iterator))
+            )
+
+            def mapper_job():
+                while not input_feeder_future.done() or not input_queue.empty():
+                    try:
+                        output_queue.put(func(input_queue.get(timeout=0.01)))
+                    except Empty:
+                        pass
+                    except Exception as e:
+                        output_queue.put(_CatchedError(e))
+
+            futures = [executor.submit(mapper_job) for _ in range(n_threads)]
+            while (
+                not all((future.done() for future in futures))
+                or not output_queue.empty()
+            ):
                 try:
-                    yield queue.get(block=False)
+                    yield output_queue.get(timeout=0.01)
                 except Empty:
-                    time.sleep(0.05)
+                    pass
+
+
+class _CatchedError:
+    def __init__(self, exception: Exception) -> None:
+        super().__init__()
+        self.exception: E = exception
+
+
+class _RasingPipe(Pipe[T]):
+    def __init__(self, iterator: Iterator[T]) -> None:
+        super().__init__(iterator)
+
+    def __next__(self) -> T:
+        next_elem = super().__next__()
+        if isinstance(next_elem, _CatchedError):
+            raise next_elem.exception
+        else:
+            return next_elem
```

