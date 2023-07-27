# Comparing `tmp/chroma-hnswlib-0.7.1.tar.gz` & `tmp/chroma-hnswlib-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chroma-hnswlib-0.7.1.tar", last modified: Mon Jul 10 19:23:00 2023, max compression
+gzip compressed data, was "chroma-hnswlib-0.7.2.tar", last modified: Thu Jul 27 17:20:49 2023, max compression
```

## Comparing `chroma-hnswlib-0.7.1.tar` & `chroma-hnswlib-0.7.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-07-10 19:23:00.296464 chroma-hnswlib-0.7.1/
--rw-r--r--   0 hammad     (501) staff       (20)    11357 2023-03-07 20:33:37.000000 chroma-hnswlib-0.7.1/LICENSE
--rw-r--r--   0 hammad     (501) staff       (20)       36 2023-03-07 20:33:37.000000 chroma-hnswlib-0.7.1/MANIFEST.in
--rw-r--r--   0 hammad     (501) staff       (20)      231 2023-07-10 19:23:00.296309 chroma-hnswlib-0.7.1/PKG-INFO
--rw-r--r--   0 hammad     (501) staff       (20)      109 2023-07-10 19:13:46.000000 chroma-hnswlib-0.7.1/README.md
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-07-10 19:23:00.294023 chroma-hnswlib-0.7.1/chroma_hnswlib.egg-info/
--rw-r--r--   0 hammad     (501) staff       (20)      231 2023-07-10 19:23:00.000000 chroma-hnswlib-0.7.1/chroma_hnswlib.egg-info/PKG-INFO
--rw-r--r--   0 hammad     (501) staff       (20)      433 2023-07-10 19:23:00.000000 chroma-hnswlib-0.7.1/chroma_hnswlib.egg-info/SOURCES.txt
--rw-r--r--   0 hammad     (501) staff       (20)        1 2023-07-10 19:23:00.000000 chroma-hnswlib-0.7.1/chroma_hnswlib.egg-info/dependency_links.txt
--rw-r--r--   0 hammad     (501) staff       (20)        1 2023-06-29 14:19:20.000000 chroma-hnswlib-0.7.1/chroma_hnswlib.egg-info/not-zip-safe
--rw-r--r--   0 hammad     (501) staff       (20)        6 2023-07-10 19:23:00.000000 chroma-hnswlib-0.7.1/chroma_hnswlib.egg-info/requires.txt
--rw-r--r--   0 hammad     (501) staff       (20)        8 2023-07-10 19:23:00.000000 chroma-hnswlib-0.7.1/chroma_hnswlib.egg-info/top_level.txt
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-07-10 19:23:00.296055 chroma-hnswlib-0.7.1/hnswlib/
--rw-r--r--   0 hammad     (501) staff       (20)     5791 2023-03-07 20:33:37.000000 chroma-hnswlib-0.7.1/hnswlib/bruteforce.h
--rw-r--r--   0 hammad     (501) staff       (20)    66429 2023-07-10 19:12:05.000000 chroma-hnswlib-0.7.1/hnswlib/hnswalg.h
--rw-r--r--   0 hammad     (501) staff       (20)     5199 2023-03-07 20:33:37.000000 chroma-hnswlib-0.7.1/hnswlib/hnswlib.h
--rw-r--r--   0 hammad     (501) staff       (20)    10855 2023-03-07 20:33:37.000000 chroma-hnswlib-0.7.1/hnswlib/space_ip.h
--rw-r--r--   0 hammad     (501) staff       (20)     8561 2023-03-07 20:33:37.000000 chroma-hnswlib-0.7.1/hnswlib/space_l2.h
--rw-r--r--   0 hammad     (501) staff       (20)     1790 2023-03-07 20:33:37.000000 chroma-hnswlib-0.7.1/hnswlib/visited_list_pool.h
--rw-r--r--   0 hammad     (501) staff       (20)      148 2023-03-07 20:33:37.000000 chroma-hnswlib-0.7.1/pyproject.toml
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-07-10 19:23:00.290136 chroma-hnswlib-0.7.1/python_bindings/
--rw-r--r--   0 hammad     (501) staff       (20)    38066 2023-07-10 19:12:05.000000 chroma-hnswlib-0.7.1/python_bindings/bindings.cpp
--rw-r--r--   0 hammad     (501) staff       (20)       38 2023-07-10 19:23:00.296512 chroma-hnswlib-0.7.1/setup.cfg
--rw-r--r--   0 hammad     (501) staff       (20)     3671 2023-07-10 19:14:10.000000 chroma-hnswlib-0.7.1/setup.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-07-27 17:20:49.894110 chroma-hnswlib-0.7.2/
+-rw-r--r--   0 hammad     (501) staff       (20)    11357 2023-03-07 20:33:37.000000 chroma-hnswlib-0.7.2/LICENSE
+-rw-r--r--   0 hammad     (501) staff       (20)       36 2023-03-07 20:33:37.000000 chroma-hnswlib-0.7.2/MANIFEST.in
+-rw-r--r--   0 hammad     (501) staff       (20)      231 2023-07-27 17:20:49.893952 chroma-hnswlib-0.7.2/PKG-INFO
+-rw-r--r--   0 hammad     (501) staff       (20)      109 2023-07-10 19:13:46.000000 chroma-hnswlib-0.7.2/README.md
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-07-27 17:20:49.888023 chroma-hnswlib-0.7.2/chroma_hnswlib.egg-info/
+-rw-r--r--   0 hammad     (501) staff       (20)      231 2023-07-27 17:20:49.000000 chroma-hnswlib-0.7.2/chroma_hnswlib.egg-info/PKG-INFO
+-rw-r--r--   0 hammad     (501) staff       (20)      433 2023-07-27 17:20:49.000000 chroma-hnswlib-0.7.2/chroma_hnswlib.egg-info/SOURCES.txt
+-rw-r--r--   0 hammad     (501) staff       (20)        1 2023-07-27 17:20:49.000000 chroma-hnswlib-0.7.2/chroma_hnswlib.egg-info/dependency_links.txt
+-rw-r--r--   0 hammad     (501) staff       (20)        1 2023-07-25 23:58:31.000000 chroma-hnswlib-0.7.2/chroma_hnswlib.egg-info/not-zip-safe
+-rw-r--r--   0 hammad     (501) staff       (20)        6 2023-07-27 17:20:49.000000 chroma-hnswlib-0.7.2/chroma_hnswlib.egg-info/requires.txt
+-rw-r--r--   0 hammad     (501) staff       (20)        8 2023-07-27 17:20:49.000000 chroma-hnswlib-0.7.2/chroma_hnswlib.egg-info/top_level.txt
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-07-27 17:20:49.893576 chroma-hnswlib-0.7.2/hnswlib/
+-rw-r--r--   0 hammad     (501) staff       (20)     5791 2023-03-07 20:33:37.000000 chroma-hnswlib-0.7.2/hnswlib/bruteforce.h
+-rw-r--r--   0 hammad     (501) staff       (20)    67355 2023-07-26 00:07:53.000000 chroma-hnswlib-0.7.2/hnswlib/hnswalg.h
+-rw-r--r--   0 hammad     (501) staff       (20)     5199 2023-03-07 20:33:37.000000 chroma-hnswlib-0.7.2/hnswlib/hnswlib.h
+-rw-r--r--   0 hammad     (501) staff       (20)    10855 2023-03-07 20:33:37.000000 chroma-hnswlib-0.7.2/hnswlib/space_ip.h
+-rw-r--r--   0 hammad     (501) staff       (20)     8561 2023-03-07 20:33:37.000000 chroma-hnswlib-0.7.2/hnswlib/space_l2.h
+-rw-r--r--   0 hammad     (501) staff       (20)     1790 2023-03-07 20:33:37.000000 chroma-hnswlib-0.7.2/hnswlib/visited_list_pool.h
+-rw-r--r--   0 hammad     (501) staff       (20)      148 2023-03-07 20:33:37.000000 chroma-hnswlib-0.7.2/pyproject.toml
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-07-27 17:20:49.882142 chroma-hnswlib-0.7.2/python_bindings/
+-rw-r--r--   0 hammad     (501) staff       (20)    38784 2023-07-26 17:27:20.000000 chroma-hnswlib-0.7.2/python_bindings/bindings.cpp
+-rw-r--r--   0 hammad     (501) staff       (20)       38 2023-07-27 17:20:49.894158 chroma-hnswlib-0.7.2/setup.cfg
+-rw-r--r--   0 hammad     (501) staff       (20)     3671 2023-07-27 17:17:15.000000 chroma-hnswlib-0.7.2/setup.py
```

### Comparing `chroma-hnswlib-0.7.1/LICENSE` & `chroma-hnswlib-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chroma-hnswlib-0.7.1/hnswlib/bruteforce.h` & `chroma-hnswlib-0.7.2/hnswlib/bruteforce.h`

 * *Files identical despite different names*

### Comparing `chroma-hnswlib-0.7.1/hnswlib/hnswalg.h` & `chroma-hnswlib-0.7.2/hnswlib/hnswalg.h`

 * *Files 3% similar despite different names*

```diff
@@ -79,14 +79,15 @@
     std::mutex elements_to_persist_lock_; // lock for elements_to_persist_
     std::set<tableint> elements_to_persist_; // dirty elements to persist
     // File handles for persistence
     std::ofstream output_header_; // output stream for header
     std::ofstream output_data_level0_; // output stream for data level 0
     std::ofstream output_length_; // output stream for length
     std::ofstream output_link_lists_; // output stream for link lists
+    bool _persist_file_handles_opened = false; // flag to check if file handles are opened
 
     HierarchicalNSW(SpaceInterface<dist_t> *s) {
     }
 
 
     HierarchicalNSW(
         SpaceInterface<dist_t> *s,
@@ -183,15 +184,15 @@
         for (tableint i = 0; i < cur_element_count; i++) {
             if (element_levels_[i] > 0)
                 free(linkLists_[i]);
         }
         free(linkLists_);
         free(length_memory_);
         delete visited_list_pool_;
-        closePersistentIndexFileHandles();
+        closePersistentIndex();
     }
 
 
     struct CompareByFirst {
         constexpr bool operator()(std::pair<dist_t, tableint> const& a,
             std::pair<dist_t, tableint> const& b) const noexcept {
             return a.first < b.first;
@@ -742,14 +743,30 @@
     void closePersistentIndexFileHandles() {
         this->output_header_.close();
         this->output_data_level0_.close();
         this->output_length_.close();
         this->output_link_lists_.close();
     }
 
+    void openPersistentIndex() {
+        // A persisted index is stored as four files, this function opens them for reading, so that calling processes can manage the file handle
+        // utilization themselves. This function is safe to repeatedly call, it will only open the files if they are not already open.
+        if (!_persist_file_handles_opened && persist_on_write_){
+            setupPersistentIndexFileHandles();
+            _persist_file_handles_opened = true;
+        }
+    }
+
+    void closePersistentIndex() {
+        if (_persist_file_handles_opened && persist_on_write_){
+            closePersistentIndexFileHandles();
+            _persist_file_handles_opened = false;
+        }
+    }
+
     void initPersistentIndex() {
         // A persisted index is stored as four files
         // The latter 3 files are stored seperately so that they can each grow as the index grows 
         // 1. The header
         // 2. The data_level_0
         // 3. length_memory_
         // 4. linkLists
@@ -780,15 +797,15 @@
         // Close file handles
         output_header.close();
         output_data_level0.close();
         output_length.close();
         output_link_lists.close();
 
         // Create file handles for further writing
-        setupPersistentIndexFileHandles();
+        openPersistentIndex();
     }
 
     void persistHeader(std::ofstream &output_header) {
         if (!persist_on_write_){
             throw std::runtime_error("persistHeader called for an index that is not set to persist on write");
         }
 
@@ -817,14 +834,18 @@
         if (elements_to_persist_.size() == 0) {
             return;
         }
 
         if (!persist_on_write_){
             throw std::runtime_error("persistDirty called for an index that is not set to persist on write");
         }
+
+        if (!_persist_file_handles_opened) {
+            throw std::runtime_error("persistDirty called for an index that has not opened its file handles");
+        }
         
         persistHeader(this->output_header_);
 
         // Note: We could benefit a lot from async IO here. Either via classic POSIX AIO or via libaio
         // Generally, this storage scheme is a bit naive, and we could do a lot better in terms of disk access patterns
         this->output_data_level0_.seekp(0, std::ios::beg);
         for (const auto& id : elements_to_persist_) {
@@ -931,15 +952,15 @@
         if (!input_link_list.is_open())
             throw std::runtime_error("Cannot open link list file");
         loadLinkLists(input_link_list);
         input_link_list.close();
 
         loadDeleted();
 
-        setupPersistentIndexFileHandles();
+        openPersistentIndex();
         return;
     }
     // #pragma endregion
 
     void loadLinkLists(std::ifstream& input_link_list) {
         // Init link lists / visited lists pool
         size_links_per_element_ = maxM_ * sizeof(tableint) + sizeof(linklistsizeint);
```

### Comparing `chroma-hnswlib-0.7.1/hnswlib/hnswlib.h` & `chroma-hnswlib-0.7.2/hnswlib/hnswlib.h`

 * *Files identical despite different names*

### Comparing `chroma-hnswlib-0.7.1/hnswlib/space_ip.h` & `chroma-hnswlib-0.7.2/hnswlib/space_ip.h`

 * *Files identical despite different names*

### Comparing `chroma-hnswlib-0.7.1/hnswlib/space_l2.h` & `chroma-hnswlib-0.7.2/hnswlib/space_l2.h`

 * *Files identical despite different names*

### Comparing `chroma-hnswlib-0.7.1/hnswlib/visited_list_pool.h` & `chroma-hnswlib-0.7.2/hnswlib/visited_list_pool.h`

 * *Files identical despite different names*

### Comparing `chroma-hnswlib-0.7.1/python_bindings/bindings.cpp` & `chroma-hnswlib-0.7.2/python_bindings/bindings.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -142,14 +142,15 @@
 }
 
 
 template<typename dist_t, typename data_t = float>
 class Index {
  public:
     static const int ser_version = 1;  // serialization version
+    static const int file_handle_count = 4; // number of file handles to open for persistent index
 
     std::string space_name;
     int dim;
     size_t seed;
     size_t default_ef;
 
     bool index_inited;
@@ -236,14 +237,26 @@
       index_inited = true;
     }
 
     void persistDirty() {
         appr_alg->persistDirty();
     }
 
+    void openFileHandles() {
+        if (!index_inited)
+            throw std::runtime_error("The index is not initiated.");
+        appr_alg->openPersistentIndex();
+    }
+
+    void closeFileHandles() {
+        if (!index_inited)
+            throw std::runtime_error("The index is not initiated.");
+        appr_alg->closePersistentIndex();
+    }
+
     void normalize_vector(float* data, float* norm_array) {
         float norm = 0.0f;
         for (int i = 0; i < dim; i++)
             norm += data[i] * data[i];
         norm = 1.0f / (sqrtf(norm) + 1e-30f);
         for (int i = 0; i < dim; i++)
             norm_array[i] = data[i] * norm;
@@ -903,14 +916,16 @@
         .def("load_index",
             &Index<float>::loadIndex,
             py::arg("path_to_index"),
             py::arg("max_elements") = 0,
             py::arg("allow_replace_deleted") = false,
             py::arg("is_persistent_index") = false)
         .def("persist_dirty", &Index<float>::persistDirty)
+        .def("open_file_handles", &Index<float>::openFileHandles)
+        .def("close_file_handles", &Index<float>::closeFileHandles)
         .def("mark_deleted", &Index<float>::markDeleted, py::arg("label"))
         .def("unmark_deleted", &Index<float>::unmarkDeleted, py::arg("label"))
         .def("resize_index", &Index<float>::resizeIndex, py::arg("new_size"))
         .def("get_max_elements", &Index<float>::getMaxElements)
         .def("get_current_count", &Index<float>::getCurrentCount)
         .def_readonly("space", &Index<float>::space_name)
         .def_readonly("dim", &Index<float>::dim)
@@ -932,15 +947,16 @@
         })
         .def_property_readonly("ef_construction", [](const Index<float> & index) {
           return index.index_inited ? index.appr_alg->ef_construction_ : 0;
         })
         .def_property_readonly("M",  [](const Index<float> & index) {
           return index.index_inited ? index.appr_alg->M_ : 0;
         })
-
+        .def_property_readonly_static("file_handle_count", [](py::object /* self */){ return Index<float>::file_handle_count; })
+        
         .def(py::pickle(
             [](const Index<float> &ind) {  // __getstate__
                 return py::make_tuple(ind.getIndexParams()); /* Return dict (wrapped in a tuple) that fully encodes state of the Index object */
             },
             [](py::tuple t) {  // __setstate__
                 if (t.size() != 1)
                     throw std::runtime_error("Invalid state!");
```

### Comparing `chroma-hnswlib-0.7.1/setup.py` & `chroma-hnswlib-0.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import numpy as np
 import pybind11
 import setuptools
 from setuptools import Extension, setup
 from setuptools.command.build_ext import build_ext
 
-__version__ = '0.7.1'
+__version__ = '0.7.2'
 
 
 include_dirs = [
     pybind11.get_include(),
     np.get_include(),
 ]
```

