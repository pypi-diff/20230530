# Comparing `tmp/hadoop_fs_wrapper-0.5.2.tar.gz` & `tmp/hadoop_fs_wrapper-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hadoop_fs_wrapper-0.5.2.tar", max compression
+gzip compressed data, was "hadoop_fs_wrapper-0.6.0.tar", max compression
```

## Comparing `hadoop_fs_wrapper-0.5.2.tar` & `hadoop_fs_wrapper-0.6.0.tar`

### file list

```diff
@@ -1,23 +1,22 @@
--rw-r--r--   0        0        0     1070 2022-11-02 12:14:52.533544 hadoop_fs_wrapper-0.5.2/LICENSE
--rw-r--r--   0        0        0     1676 2022-11-02 12:14:52.533544 hadoop_fs_wrapper-0.5.2/README.md
--rw-r--r--   0        0        0     1182 2022-11-02 12:14:52.533544 hadoop_fs_wrapper-0.5.2/hadoop_fs_wrapper/__init__.py
--rw-r--r--   0        0        0       22 2022-11-02 12:15:06.301656 hadoop_fs_wrapper-0.5.2/hadoop_fs_wrapper/_version.py
--rw-r--r--   0        0        0     1108 2022-11-02 12:14:52.533544 hadoop_fs_wrapper-0.5.2/hadoop_fs_wrapper/models/__init__.py
--rw-r--r--   0        0        0     1865 2022-11-02 12:14:52.533544 hadoop_fs_wrapper-0.5.2/hadoop_fs_wrapper/models/buffered_input_stream.py
--rw-r--r--   0        0        0     2728 2022-11-02 12:14:52.533544 hadoop_fs_wrapper-0.5.2/hadoop_fs_wrapper/models/buffered_output_stream.py
--rw-r--r--   0        0        0     1714 2022-11-02 12:14:52.533544 hadoop_fs_wrapper-0.5.2/hadoop_fs_wrapper/models/buffered_reader.py
--rw-r--r--   0        0        0     2514 2022-11-02 12:14:52.533544 hadoop_fs_wrapper-0.5.2/hadoop_fs_wrapper/models/file_status.py
--rw-r--r--   0        0        0     1387 2022-11-02 12:14:52.533544 hadoop_fs_wrapper-0.5.2/hadoop_fs_wrapper/models/fs_data_input_stream.py
--rw-r--r--   0        0        0     1390 2022-11-02 12:14:52.533544 hadoop_fs_wrapper-0.5.2/hadoop_fs_wrapper/models/fs_data_output_stream.py
--rw-r--r--   0        0        0     1684 2022-11-02 12:14:52.533544 hadoop_fs_wrapper-0.5.2/hadoop_fs_wrapper/models/glob_filter.py
--rw-r--r--   0        0        0     2523 2022-11-02 12:14:52.533544 hadoop_fs_wrapper-0.5.2/hadoop_fs_wrapper/models/hadoop_file_status.py
--rw-r--r--   0        0        0     1725 2022-11-02 12:14:52.533544 hadoop_fs_wrapper-0.5.2/hadoop_fs_wrapper/models/hadoop_fs_path.py
--rw-r--r--   0        0        0     2227 2022-11-02 12:14:52.533544 hadoop_fs_wrapper-0.5.2/hadoop_fs_wrapper/models/input_stream_reader.py
--rw-r--r--   0        0        0     2131 2022-11-02 12:14:52.533544 hadoop_fs_wrapper-0.5.2/hadoop_fs_wrapper/models/remote_iterator.py
--rw-r--r--   0        0        0     1628 2022-11-02 12:14:52.533544 hadoop_fs_wrapper-0.5.2/hadoop_fs_wrapper/models/uri.py
--rw-r--r--   0        0        0     1108 2022-11-02 12:14:52.533544 hadoop_fs_wrapper-0.5.2/hadoop_fs_wrapper/wrappers/__init__.py
--rw-r--r--   0        0        0     7015 2022-11-02 12:14:52.533544 hadoop_fs_wrapper-0.5.2/hadoop_fs_wrapper/wrappers/file_system.py
--rw-r--r--   0        0        0    11969 2022-11-02 12:14:52.533544 hadoop_fs_wrapper-0.5.2/hadoop_fs_wrapper/wrappers/hadoop_fs_wrapper.py
--rw-r--r--   0        0        0      569 2022-11-02 12:15:06.301656 hadoop_fs_wrapper-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     2475 1970-01-01 00:00:00.000000 hadoop_fs_wrapper-0.5.2/setup.py
--rw-r--r--   0        0        0     2397 1970-01-01 00:00:00.000000 hadoop_fs_wrapper-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-30 14:28:33.721819 hadoop_fs_wrapper-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1925 2023-05-30 14:28:33.721819 hadoop_fs_wrapper-0.6.0/README.md
+-rw-r--r--   0        0        0     1182 2023-05-30 14:28:33.721819 hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/__init__.py
+-rw-r--r--   0        0        0       22 2023-05-30 14:28:49.302048 hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/_version.py
+-rw-r--r--   0        0        0     1108 2023-05-30 14:28:33.721819 hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/models/__init__.py
+-rw-r--r--   0        0        0     1863 2023-05-30 14:28:33.721819 hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/models/buffered_input_stream.py
+-rw-r--r--   0        0        0     2726 2023-05-30 14:28:33.721819 hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/models/buffered_output_stream.py
+-rw-r--r--   0        0        0     1712 2023-05-30 14:28:33.721819 hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/models/buffered_reader.py
+-rw-r--r--   0        0        0     2505 2023-05-30 14:28:33.721819 hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/models/file_status.py
+-rw-r--r--   0        0        0     1385 2023-05-30 14:28:33.721819 hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/models/fs_data_input_stream.py
+-rw-r--r--   0        0        0     1388 2023-05-30 14:28:33.721819 hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/models/fs_data_output_stream.py
+-rw-r--r--   0        0        0     1682 2023-05-30 14:28:33.721819 hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/models/glob_filter.py
+-rw-r--r--   0        0        0     2493 2023-05-30 14:28:33.721819 hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/models/hadoop_file_status.py
+-rw-r--r--   0        0        0     1720 2023-05-30 14:28:33.721819 hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/models/hadoop_fs_path.py
+-rw-r--r--   0        0        0     2226 2023-05-30 14:28:33.721819 hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/models/input_stream_reader.py
+-rw-r--r--   0        0        0     2120 2023-05-30 14:28:33.721819 hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/models/remote_iterator.py
+-rw-r--r--   0        0        0     1626 2023-05-30 14:28:33.721819 hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/models/uri.py
+-rw-r--r--   0        0        0     1108 2023-05-30 14:28:33.721819 hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/wrappers/__init__.py
+-rw-r--r--   0        0        0     7060 2023-05-30 14:28:33.721819 hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/wrappers/file_system.py
+-rw-r--r--   0        0        0    11783 2023-05-30 14:28:33.721819 hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/wrappers/hadoop_fs_wrapper.py
+-rw-r--r--   0        0        0      628 2023-05-30 14:28:49.302048 hadoop_fs_wrapper-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2647 1970-01-01 00:00:00.000000 hadoop_fs_wrapper-0.6.0/PKG-INFO
```

### Comparing `hadoop_fs_wrapper-0.5.2/LICENSE` & `hadoop_fs_wrapper-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hadoop_fs_wrapper-0.5.2/README.md` & `hadoop_fs_wrapper-0.6.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 # Hadoop FileSystem Java Class Wrapper 
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
 Typed Python wrappers for [Hadoop FileSystem](https://hadoop.apache.org/docs/stable/api/org/apache/hadoop/fs/FileSystem.html) class family.
 
 ## Installation
 You can install this package from `pypi` on any Hadoop or Spark runtime:
 ```commandline
 pip install hadoop-fs-wrapper
 ```
 
 Select a version that matches hadoop version you are using:
 
-| Hadoop Version | Compatible hadoop-fs-wrapper version |
-|----------------|:------------------------------------:|
-| 3.2.x          |                0.4.x                 |
-| 3.3.x          |             0.4.x, 0.5.x             |
+| Hadoop Version / Spark version | Compatible hadoop-fs-wrapper version |
+|--------------------------------|:------------------------------------:|
+| 3.2.x / 3.2.x                  |                0.4.x                 |
+| 3.3.x / 3.3.x                  |             0.4.x, 0.5.x             |
+| 3.3.x / 3.4.x                  |                0.6.x                 |
 
 ## Usage
 Common use case is accessing Hadoop FileSystem from Spark session object:
 
 ```python
 from hadoop_fs_wrapper.wrappers.file_system import FileSystem
 
@@ -38,8 +41,8 @@
 ```
 
 ## Contribution
 
 Currently basic filesystem operations (listing, deleting, search, iterative listing etc.) are supported. If an operation you require is not yet wrapped,
 please open an issue or create a PR.
 
-All changes are tested against Spark 3.2/3.3 running in local mode.
+All changes are tested against Spark 3.4 running in local mode.
```

### Comparing `hadoop_fs_wrapper-0.5.2/hadoop_fs_wrapper/__init__.py` & `hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `hadoop_fs_wrapper-0.5.2/hadoop_fs_wrapper/models/__init__.py` & `hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hadoop_fs_wrapper-0.5.2/hadoop_fs_wrapper/models/buffered_input_stream.py` & `hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/models/buffered_input_stream.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,19 +23,20 @@
 """
   Wrapper for java.io.BufferedInputStream
 """
 
 
 class BufferedInputStream:
     """
-      Wrapper for java.io.BufferedInputStream
+    Wrapper for java.io.BufferedInputStream
     """
+
     def __init__(self, underlying):
         """
-         Class init
+        Class init
         """
         self.underlying = underlying
 
     @classmethod
     def from_input_stream(cls, jvm, input_stream):
         """
          Wraps constructor java.io.BufferedInputStream(InputStream in)
```

### Comparing `hadoop_fs_wrapper-0.5.2/hadoop_fs_wrapper/models/buffered_output_stream.py` & `hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/models/buffered_output_stream.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,19 +23,20 @@
 """
   Wrapper for java.io.BufferedOutputStream
 """
 
 
 class BufferedOutputStream:
     """
-      Wrapper for java.io.BufferedOutputStream
+    Wrapper for java.io.BufferedOutputStream
     """
+
     def __init__(self, underlying):
         """
-         Class init
+        Class init
         """
         self.underlying = underlying
 
     def write(self, data):
         """
          Wraps write(data) method.
          Writes the specified byte to this buffered output stream.
```

### Comparing `hadoop_fs_wrapper-0.5.2/hadoop_fs_wrapper/models/buffered_reader.py` & `hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/models/buffered_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,19 +23,20 @@
 """
   Wrapper for java.io.BufferedReader
 """
 
 
 class BufferedReader:
     """
-      Wrapper for java.io.BufferedReader
+    Wrapper for java.io.BufferedReader
     """
+
     def __init__(self, underlying):
         """
-         Class init
+        Class init
         """
         self.underlying = underlying
 
     @classmethod
     def from_reader(cls, jvm, reader):
         """
          Wraps constructor java.io.BufferedReader(Reader in)
```

### Comparing `hadoop_fs_wrapper-0.5.2/hadoop_fs_wrapper/models/file_status.py` & `hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/models/file_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,70 +23,71 @@
 """
  Wrapper for org.apache.hadoop.fs.FileStatus
 """
 
 
 class FileStatus:
     """
-     Wrapper for org.apache.hadoop.fs.FileStatus
+    Wrapper for org.apache.hadoop.fs.FileStatus
     """
+
     def __init__(self, underlying):
         """
-         Class init
+        Class init
         """
         self.underlying = underlying
 
     def get_path(self) -> str:
         """
-         Wraps getPath() method.
+        Wraps getPath() method.
 
         """
         return self.underlying.getPath().toString()
 
     def get_owner(self) -> str:
         """
-         Wraps getOwner() method.
+        Wraps getOwner() method.
 
         """
         return self.underlying.getOwner()
 
     def get_group(self) -> str:
         """
-         Wraps getGroup() method.
+        Wraps getGroup() method.
 
         """
         return self.underlying.getGroup()
 
     def get_permission(self) -> str:
         """
-         Wraps getPermission() method.
+        Wraps getPermission() method.
 
         """
         return self.underlying.getPermission().toString()
 
     def get_modification_time(self) -> int:
         """
-         Wraps getModificationTime() method.
+        Wraps getModificationTime() method.
 
         """
         return self.underlying.getModificationTime()
 
     def is_file(self) -> bool:
         """
-         Wraps isFile() method.
+        Wraps isFile() method.
 
         """
         return self.underlying.isFile()
 
     def get_block_size(self) -> int:
         """
-         Wraps getBlockSize() method.
+        Wraps getBlockSize() method.
 
         """
         return self.underlying.getBlockSize()
 
     def get_file_length(self) -> int:
         """
-         Wraps getLen() method.
+        Wraps getLen() method.
 
         """
         return self.underlying.getLen()
```

### Comparing `hadoop_fs_wrapper-0.5.2/hadoop_fs_wrapper/models/fs_data_input_stream.py` & `hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/models/fs_data_input_stream.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 """
   Wrapper for org.apache.hadoop.fs.FSDataInputStream
 """
 
 
 class FSDataInputStream:
     """
-      Wrapper for org.apache.hadoop.fs.FSDataInputStream
+    Wrapper for org.apache.hadoop.fs.FSDataInputStream
     """
+
     def __init__(self, underlying):
         """
-         Class init
+        Class init
         """
         self.underlying = underlying
```

### Comparing `hadoop_fs_wrapper-0.5.2/hadoop_fs_wrapper/models/fs_data_output_stream.py` & `hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/models/fs_data_output_stream.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 """
   Wrapper for org.apache.hadoop.fs.FSDataOutputStream
 """
 
 
 class FSDataOutputStream:
     """
-      Wrapper for org.apache.hadoop.fs.FSDataOutputStream
+    Wrapper for org.apache.hadoop.fs.FSDataOutputStream
     """
+
     def __init__(self, underlying):
         """
-         Class init
+        Class init
         """
         self.underlying = underlying
```

### Comparing `hadoop_fs_wrapper-0.5.2/hadoop_fs_wrapper/models/glob_filter.py` & `hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/models/glob_filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,19 +23,20 @@
 """
   Wrapper for org.apache.hadoop.fs.GlobFilter
 """
 
 
 class GlobFilter:
     """
-      Wrapper for org.apache.hadoop.fs.GlobFilter
+    Wrapper for org.apache.hadoop.fs.GlobFilter
     """
+
     def __init__(self, underlying):
         """
-         Class init
+        Class init
         """
         self.underlying = underlying
 
     @classmethod
     def from_string(cls, jvm, file_pattern: str):
         """
          Wraps GlobFilter(String filePattern):
```

### Comparing `hadoop_fs_wrapper-0.5.2/hadoop_fs_wrapper/models/hadoop_file_status.py` & `hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/models/hadoop_file_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,16 +29,17 @@
 
 from hadoop_fs_wrapper.models.file_status import FileStatus
 
 
 @dataclass
 class HadoopFileStatus:
     """
-      Interface that represents the client side information for a file.
+    Interface that represents the client side information for a file.
     """
+
     path: str
     owner: str
     group: str
     permission: str
     modified_on: datetime
     type: str
     block_size: int
@@ -53,16 +54,14 @@
         :return: object of type HadoopFileStatus
         """
         return cls(
             path=hadoop_file_status.get_path(),
             owner=hadoop_file_status.get_owner(),
             group=hadoop_file_status.get_group(),
             permission=hadoop_file_status.get_permission(),
-            modified_on=datetime.utcfromtimestamp(
-                hadoop_file_status.get_modification_time() // 1000
-            ).replace(
+            modified_on=datetime.utcfromtimestamp(hadoop_file_status.get_modification_time() // 1000).replace(
                 microsecond=hadoop_file_status.get_modification_time() % 1000 * 1000
             ),
             type="File" if hadoop_file_status.is_file() else "Folder",
             block_size=hadoop_file_status.get_block_size(),
-            length=hadoop_file_status.get_file_length()
+            length=hadoop_file_status.get_file_length(),
         )
```

### Comparing `hadoop_fs_wrapper-0.5.2/hadoop_fs_wrapper/models/hadoop_fs_path.py` & `hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/models/hadoop_fs_path.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,27 +23,28 @@
 """
   Wrapper for org.apache.hadoop.fs.Path
 """
 
 
 class HadoopFsPath:
     """
-      Wrapper for org.apache.hadoop.fs.Path
+    Wrapper for org.apache.hadoop.fs.Path
     """
+
     def __init__(self, underlying):
         """
-         Class init
+        Class init
         """
         self.underlying = underlying
 
     def uri(self):
         """
-         Returns java.net.Uri corresponding to the supplied path
+        Returns java.net.Uri corresponding to the supplied path
         """
         return self.underlying.toUri()
 
     @classmethod
     def from_string(cls, jvm, path_string: str):
         """
-          Creates a new class instance directly from a path string
+        Creates a new class instance directly from a path string
         """
         return cls(jvm.org.apache.hadoop.fs.Path(path_string))
```

### Comparing `hadoop_fs_wrapper-0.5.2/hadoop_fs_wrapper/models/input_stream_reader.py` & `hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/models/input_stream_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,32 +23,33 @@
 """
   Wrapper for java.io.InputStreamReader
 """
 
 
 class InputStreamReader:
     """
-      Wrapper for java.io.InputStreamReader
+    Wrapper for java.io.InputStreamReader
     """
+
     def __init__(self, underlying):
         """
-         Class init
+        Class init
         """
         self.underlying = underlying
 
     @classmethod
     def from_input_stream_and_charset(cls, jvm, input_stream, charset_name):
         """
          Wraps constructor java.io.InputStreamReader(InputStream in, String charsetName)
          Creates an InputStreamReader that uses the named charset.
         :param input_stream: An InputStream
         :param charset_name: The name of a supported charset
         :return: InputStreamReader
         """
-        return cls(jvm.java.io.InputStreamReader(input_stream,charset_name))
+        return cls(jvm.java.io.InputStreamReader(input_stream, charset_name))
 
     @classmethod
     def from_input_stream(cls, jvm, input_stream):
         """
          Wraps constructor java.io.InputStreamReader(InputStream in)
          Creates an InputStreamReader that uses the default charset.
         :param input_stream: An InputStream
```

### Comparing `hadoop_fs_wrapper-0.5.2/hadoop_fs_wrapper/models/remote_iterator.py` & `hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/models/remote_iterator.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,45 +21,45 @@
 # SOFTWARE.
 
 """
      Wrapper for org.apache.hadoop.fs.RemoteIterator<T>
 """
 from typing import Generic, TypeVar, Iterable, Iterator
 
-T = TypeVar('T')  # pylint: disable=C0103
+T = TypeVar("T")  # pylint: disable=C0103
 
 
 class RemoteIterator(Generic[T], Iterable[T]):
     """
-     Wrapper for org.apache.hadoop.fs.RemoteIterator<T>
+    Wrapper for org.apache.hadoop.fs.RemoteIterator<T>
     """
 
     def __iter__(self) -> Iterator[T]:
         return self
 
     def __init__(self, underlying):
         """
-         Class init
+        Class init
         """
         self.underlying = underlying
 
     def _next(self) -> T:
         """
-         Wraps E next()
-               throws IOException
-               Returns the next element in the iteration.
+        Wraps E next()
+              throws IOException
+              Returns the next element in the iteration.
         """
 
         return self.underlying.next()
 
     def _has_next(self) -> bool:
         """
-          Wraps boolean hasNext()
-                throws IOException
-                Returns true if the iteration has more elements.
+        Wraps boolean hasNext()
+              throws IOException
+              Returns true if the iteration has more elements.
         """
 
         return self.underlying.hasNext()
 
     def __next__(self) -> T:
         if self._has_next():
             return self._next()
```

### Comparing `hadoop_fs_wrapper-0.5.2/hadoop_fs_wrapper/models/uri.py` & `hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/models/uri.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,19 +23,20 @@
 """
   Wrapper for java.net.URI
 """
 
 
 class URI:
     """
-      Wrapper for java.net.URI
+    Wrapper for java.net.URI
     """
+
     def __init__(self, underlying):
         """
-         Class init
+        Class init
         """
         self.underlying = underlying
 
     @classmethod
     def from_string(cls, jvm, uri_str):
         """
          Wraps constructor java.net.URI(String str)
```

### Comparing `hadoop_fs_wrapper-0.5.2/hadoop_fs_wrapper/wrappers/__init__.py` & `hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `hadoop_fs_wrapper-0.5.2/hadoop_fs_wrapper/wrappers/file_system.py` & `hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/wrappers/file_system.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,16 @@
 from hadoop_fs_wrapper.wrappers.hadoop_fs_wrapper import HadoopFsWrapper
 from hadoop_fs_wrapper.models.hadoop_file_status import HadoopFileStatus
 from hadoop_fs_wrapper.models.file_status import FileStatus
 
 
 class FileSystem:
     """
-      Wrapper around Hadoop FileSystem (Java)
-      https://hadoop.apache.org/docs/stable/api/org/apache/hadoop/fs/FileSystem.html
+    Wrapper around Hadoop FileSystem (Java)
+    https://hadoop.apache.org/docs/stable/api/org/apache/hadoop/fs/FileSystem.html
     """
 
     def __init__(self, jvm, conf):
         self._jvm = jvm
         self._conf = conf
         self._fsw = HadoopFsWrapper(jvm=self._jvm, conf=self._conf)
 
@@ -57,32 +57,35 @@
          Filter files/directories in the given path using the user-supplied path filter.
          Does not guarantee to return the List of files/directories status in a sorted order.
         :param path: a path name
         :param globfilter: the user-supplied path globfilter
         :return: List of type HadoopFileStatus
         """
         fs_path = self._fsw.path(path)
-        files = self._fsw.list_status(fs_path) if not globfilter \
+        files = (
+            self._fsw.list_status(fs_path)
+            if not globfilter
             else self._fsw.list_status_filter(fs_path, self._fsw.glob_filter(globfilter))
+        )
 
         if files:
             return list(map(HadoopFileStatus.from_file_status, files))
 
         return []
 
     def list_objects_stream(self, *, path: str) -> Iterator[HadoopFileStatus]:
         """
-         Returns a remote iterator so that followup calls are made on demand while consuming the entries.
-         Each Hadoop FileSystem implementation should override this method and provide a more efficient implementation, if possible.
-         Does not guarantee to return the iterator that traverses statuses of the files in a sorted order.
+        Returns a remote iterator so that followup calls are made on demand while consuming the entries.
+        Each Hadoop FileSystem implementation should override this method and provide a more efficient implementation, if possible.
+        Does not guarantee to return the iterator that traverses statuses of the files in a sorted order.
 
-         https://hadoop.apache.org/docs/stable/api/org/apache/hadoop/fs/FileSystem.html#listStatusIterator-org.apache.hadoop.fs.Path-
+        https://hadoop.apache.org/docs/stable/api/org/apache/hadoop/fs/FileSystem.html#listStatusIterator-org.apache.hadoop.fs.Path-
 
-         :param path: Path to list objects in.
-         :return: Iterator of HadoopFileStatus objects
+        :param path: Path to list objects in.
+        :return: Iterator of HadoopFileStatus objects
         """
         fs_path = self._fsw.path(path)
         fs_iterator = self._fsw.list_status_iterator(path=fs_path)
         for fs_obj in fs_iterator:
             yield HadoopFileStatus.from_file_status(FileStatus(fs_obj))
 
     def glob_status(self, path_pattern: str, globfilter: str = None) -> List[HadoopFileStatus]:
@@ -91,16 +94,19 @@
          and is accepted by the user-supplied path filter.
          Results are sorted by their path names.
         :param path_pattern: a glob specifying the path pattern
         :param globfilter: a user-supplied path filter
         :return: List of type HadoopFileStatus
         """
         fs_path = self._fsw.path(path_pattern)
-        files = self._fsw.glob_status(fs_path) if not globfilter \
+        files = (
+            self._fsw.glob_status(fs_path)
+            if not globfilter
             else self._fsw.glob_status_filter(fs_path, self._fsw.glob_filter(globfilter))
+        )
 
         if files:
             return list(map(HadoopFileStatus.from_file_status, files))
 
         return []
 
     def delete(self, path: str, recursive: bool = False) -> bool:
@@ -129,15 +135,15 @@
          un-renamed
         :param src: path to be renamed
         :param dst: new path after rename
         :return: True if rename is successful
         """
         return self._fsw.rename(self._fsw.path(src), self._fsw.path(dst))
 
-    def write(self, path: str, data: str, overwrite=False, encoding='utf-8'):
+    def write(self, path: str, data: str, overwrite=False, encoding="utf-8"):
         """
          Writes stringdata to a new file with optional overwrite
         :param path: path to write to
         :param data: stringdata to write
         :param overwrite: if a file with this name already exists,
                           then if true, the file will be overwritten,
                           and if false an exception will be thrown.
@@ -145,21 +151,20 @@
         :return:
         """
         stream = self._fsw.create(self._fsw.path(path), overwrite)
         buffered_stream = self._fsw.buffered_output_stream(stream)
         buffered_stream.write(data.encode(encoding))
         buffered_stream.close()
 
-    def read(self, path: str, encoding='utf-8') -> str:
+    def read(self, path: str, encoding="utf-8") -> str:
         """
          reads stringdata from file
         :param path: path to read
         :param encoding: encoding to read
         :return: string
         """
         stream = self._fsw.open(self._fsw.path(path))
         buffered_stream = self._fsw.buffered_input_stream(stream)
-        input_stream_reader = self._fsw.input_stream_reader(
-            buffered_stream, encoding)
+        input_stream_reader = self._fsw.input_stream_reader(buffered_stream, encoding)
         buffered_reader = self._fsw.buffered_reader(input_stream_reader)
-        lines_collector = self._jvm.java.util.stream.Collectors.joining('\n')
+        lines_collector = self._jvm.java.util.stream.Collectors.joining("\n")
         return buffered_reader.underlying.lines().collect(lines_collector)
```

### Comparing `hadoop_fs_wrapper-0.5.2/hadoop_fs_wrapper/wrappers/hadoop_fs_wrapper.py` & `hadoop_fs_wrapper-0.6.0/hadoop_fs_wrapper/wrappers/hadoop_fs_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,16 +36,16 @@
 from hadoop_fs_wrapper.models.buffered_input_stream import BufferedInputStream
 from hadoop_fs_wrapper.models.glob_filter import GlobFilter
 from hadoop_fs_wrapper.models.input_stream_reader import InputStreamReader
 
 
 class HadoopFsWrapper:
     """
-      Wrapper around Hadoop FileSystem (Java)
-      https://hadoop.apache.org/docs/stable/api/org/apache/hadoop/fs/FileSystem.html
+    Wrapper around Hadoop FileSystem (Java)
+    https://hadoop.apache.org/docs/stable/api/org/apache/hadoop/fs/FileSystem.html
     """
 
     def __init__(self, jvm, conf):
         self._jvm = jvm
         self._conf = conf
 
     def delete(self, path: HadoopFsPath, recursive: bool = True) -> bool:
@@ -242,30 +242,26 @@
          Creates a buffering character-input stream that
          uses a default-sized input buffer.
         :param input_reader: A Reader
         :return: BufferedReader
         """
         return BufferedReader.from_reader(self._jvm, input_reader.underlying)
 
-    def input_stream_reader(self,
-                            input_stream: InputStreamReader,
-                            charset_name: str = None) -> InputStreamReader:
+    def input_stream_reader(self, input_stream: InputStreamReader, charset_name: str = None) -> InputStreamReader:
         """
           Wraps constructor java.io.InputStreamReader(InputStream in)
           Creates an InputStreamReader that uses the named charset.
 
         :param input_stream: An InputStream
         :param charset_name: The name of a supported charset
         :return: InputStreamReader
         """
         if not charset_name:
             return InputStreamReader.from_input_stream(self._jvm, input_stream.underlying)
-        return InputStreamReader.from_input_stream_and_charset(self._jvm,
-                                                               input_stream.underlying,
-                                                               charset_name)
+        return InputStreamReader.from_input_stream_and_charset(self._jvm, input_stream.underlying, charset_name)
 
     def list_status_iterator(self, path: HadoopFsPath) -> RemoteIterator[FileStatus]:
         """
           Wraps public org.apache.hadoop.fs.RemoteIterator<FileStatus> listStatusIterator(Path p)
              throws FileNotFoundException,
              IOException
```

### Comparing `hadoop_fs_wrapper-0.5.2/pyproject.toml` & `hadoop_fs_wrapper-0.6.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 [tool.poetry]
 name = "hadoop-fs-wrapper"
-version = "0.5.2"
+version = "0.6.0"
 description = "Python Wrapper for Hadoop Java API"
 authors = ["ECCO Sneaks & Data <esdsupport@ecco.com>"]
 maintainers = ['GZU <gzu@ecco.com>', 'JRB <ext-jrb@ecco.com>']
 license = 'MIT'
 readme = "README.md"
 repository = 'https://github.com/SneaksAndData/hadoop-fs-wrapper'
 
 [tool.poetry.dependencies]
-python = "^3.9"
-pyspark = "~3.3"
+python = ">=3.9, <3.12"
+pyspark = "~3.4"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.0"
 pytest-cov = "^3.0"
 pylint = "^2.12"
+black = "~22.12.0"
 
 [build-system]
 requires = ["poetry-core>=1.2.0"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.black]
+line-length = 120
```

### Comparing `hadoop_fs_wrapper-0.5.2/setup.py` & `hadoop_fs_wrapper-0.6.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,69 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: hadoop-fs-wrapper
+Version: 0.6.0
+Summary: Python Wrapper for Hadoop Java API
+Home-page: https://github.com/SneaksAndData/hadoop-fs-wrapper
+License: MIT
+Author: ECCO Sneaks & Data
+Author-email: esdsupport@ecco.com
+Maintainer: GZU
+Maintainer-email: gzu@ecco.com
+Requires-Python: >=3.9,<3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pyspark (>=3.4,<3.5)
+Project-URL: Repository, https://github.com/SneaksAndData/hadoop-fs-wrapper
+Description-Content-Type: text/markdown
+
+# Hadoop FileSystem Java Class Wrapper 
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+Typed Python wrappers for [Hadoop FileSystem](https://hadoop.apache.org/docs/stable/api/org/apache/hadoop/fs/FileSystem.html) class family.
+
+## Installation
+You can install this package from `pypi` on any Hadoop or Spark runtime:
+```commandline
+pip install hadoop-fs-wrapper
+```
+
+Select a version that matches hadoop version you are using:
+
+| Hadoop Version / Spark version | Compatible hadoop-fs-wrapper version |
+|--------------------------------|:------------------------------------:|
+| 3.2.x / 3.2.x                  |                0.4.x                 |
+| 3.3.x / 3.3.x                  |             0.4.x, 0.5.x             |
+| 3.3.x / 3.4.x                  |                0.6.x                 |
+
+## Usage
+Common use case is accessing Hadoop FileSystem from Spark session object:
+
+```python
+from hadoop_fs_wrapper.wrappers.file_system import FileSystem
+
+file_system = FileSystem.from_spark_session(spark=spark_session)
+```
+
+Then, for example, one can check if there are any files under specified path:
+```python
+from hadoop_fs_wrapper.wrappers.file_system import FileSystem
+
+def is_valid_source_path(file_system: FileSystem, path: str) -> bool:
+    """
+     Checks whether a regexp path refers to a valid set of paths
+    :param file_system: pyHadooopWrapper FileSystem
+    :param path: path e.g. (s3a|abfss|file|...)://hello@world.com/path/part*.csv
+    :return: true if path resolves to existing paths, otherwise false
+    """
+    return len(file_system.glob_status(path)) > 0
+```
 
-packages = \
-['hadoop_fs_wrapper', 'hadoop_fs_wrapper.models', 'hadoop_fs_wrapper.wrappers']
+## Contribution
 
-package_data = \
-{'': ['*']}
+Currently basic filesystem operations (listing, deleting, search, iterative listing etc.) are supported. If an operation you require is not yet wrapped,
+please open an issue or create a PR.
 
-install_requires = \
-['pyspark>=3.3,<3.4']
-
-setup_kwargs = {
-    'name': 'hadoop-fs-wrapper',
-    'version': '0.5.2',
-    'description': 'Python Wrapper for Hadoop Java API',
-    'long_description': '# Hadoop FileSystem Java Class Wrapper \nTyped Python wrappers for [Hadoop FileSystem](https://hadoop.apache.org/docs/stable/api/org/apache/hadoop/fs/FileSystem.html) class family.\n\n## Installation\nYou can install this package from `pypi` on any Hadoop or Spark runtime:\n```commandline\npip install hadoop-fs-wrapper\n```\n\nSelect a version that matches hadoop version you are using:\n\n| Hadoop Version | Compatible hadoop-fs-wrapper version |\n|----------------|:------------------------------------:|\n| 3.2.x          |                0.4.x                 |\n| 3.3.x          |             0.4.x, 0.5.x             |\n\n## Usage\nCommon use case is accessing Hadoop FileSystem from Spark session object:\n\n```python\nfrom hadoop_fs_wrapper.wrappers.file_system import FileSystem\n\nfile_system = FileSystem.from_spark_session(spark=spark_session)\n```\n\nThen, for example, one can check if there are any files under specified path:\n```python\nfrom hadoop_fs_wrapper.wrappers.file_system import FileSystem\n\ndef is_valid_source_path(file_system: FileSystem, path: str) -> bool:\n    """\n     Checks whether a regexp path refers to a valid set of paths\n    :param file_system: pyHadooopWrapper FileSystem\n    :param path: path e.g. (s3a|abfss|file|...)://hello@world.com/path/part*.csv\n    :return: true if path resolves to existing paths, otherwise false\n    """\n    return len(file_system.glob_status(path)) > 0\n```\n\n## Contribution\n\nCurrently basic filesystem operations (listing, deleting, search, iterative listing etc.) are supported. If an operation you require is not yet wrapped,\nplease open an issue or create a PR.\n\nAll changes are tested against Spark 3.2/3.3 running in local mode.',
-    'author': 'ECCO Sneaks & Data',
-    'author_email': 'esdsupport@ecco.com',
-    'maintainer': 'GZU',
-    'maintainer_email': 'gzu@ecco.com',
-    'url': 'https://github.com/SneaksAndData/hadoop-fs-wrapper',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
-}
+All changes are tested against Spark 3.4 running in local mode.
 
-
-setup(**setup_kwargs)
```

