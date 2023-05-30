# Comparing `tmp/somacore-1.0.2.tar.gz` & `tmp/somacore-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "somacore-1.0.2.tar", last modified: Wed Apr 26 14:47:47 2023, max compression
+gzip compressed data, was "somacore-1.0.3.tar", last modified: Tue May 30 16:36:36 2023, max compression
```

## Comparing `somacore-1.0.2.tar` & `somacore-1.0.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:47:47.685483 somacore-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-26 14:47:17.000000 somacore-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-26 14:47:17.000000 somacore-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-26 14:47:47.685483 somacore-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-26 14:47:17.000000 somacore-1.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:47:47.685483 somacore-1.0.2/python-spec/
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-26 14:47:17.000000 somacore-1.0.2/python-spec/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:47:47.681483 somacore-1.0.2/python-spec/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:47:47.685483 somacore-1.0.2/python-spec/src/somacore/
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-26 14:47:17.000000 somacore-1.0.2/python-spec/src/somacore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-26 14:47:17.000000 somacore-1.0.2/python-spec/src/somacore/_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-26 14:47:47.000000 somacore-1.0.2/python-spec/src/somacore/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-04-26 14:47:17.000000 somacore-1.0.2/python-spec/src/somacore/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8891 2023-04-26 14:47:17.000000 somacore-1.0.2/python-spec/src/somacore/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    19796 2023-04-26 14:47:17.000000 somacore-1.0.2/python-spec/src/somacore/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:47:47.685483 somacore-1.0.2/python-spec/src/somacore/ephemeral/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-26 14:47:17.000000 somacore-1.0.2/python-spec/src/somacore/ephemeral/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-04-26 14:47:17.000000 somacore-1.0.2/python-spec/src/somacore/ephemeral/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-04-26 14:47:17.000000 somacore-1.0.2/python-spec/src/somacore/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-04-26 14:47:17.000000 somacore-1.0.2/python-spec/src/somacore/measurement.py
--rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-04-26 14:47:17.000000 somacore-1.0.2/python-spec/src/somacore/options.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-26 14:47:17.000000 somacore-1.0.2/python-spec/src/somacore/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:47:47.685483 somacore-1.0.2/python-spec/src/somacore/query/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-26 14:47:17.000000 somacore-1.0.2/python-spec/src/somacore/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-26 14:47:17.000000 somacore-1.0.2/python-spec/src/somacore/query/_eager_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-04-26 14:47:17.000000 somacore-1.0.2/python-spec/src/somacore/query/_fast_csr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-04-26 14:47:17.000000 somacore-1.0.2/python-spec/src/somacore/query/axis.py
--rw-r--r--   0 runner    (1001) docker     (123)    18156 2023-04-26 14:47:17.000000 somacore-1.0.2/python-spec/src/somacore/query/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-04-26 14:47:17.000000 somacore-1.0.2/python-spec/src/somacore/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:47:47.685483 somacore-1.0.2/python-spec/src/somacore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-26 14:47:47.000000 somacore-1.0.2/python-spec/src/somacore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 14:47:47.685483 somacore-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:36:36.585210 somacore-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-30 16:36:16.000000 somacore-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-30 16:36:16.000000 somacore-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-30 16:36:36.585210 somacore-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-30 16:36:16.000000 somacore-1.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:36:36.585210 somacore-1.0.3/python-spec/
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-30 16:36:16.000000 somacore-1.0.3/python-spec/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:36:36.581210 somacore-1.0.3/python-spec/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:36:36.585210 somacore-1.0.3/python-spec/src/somacore/
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-30 16:36:16.000000 somacore-1.0.3/python-spec/src/somacore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-30 16:36:16.000000 somacore-1.0.3/python-spec/src/somacore/_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-30 16:36:36.000000 somacore-1.0.3/python-spec/src/somacore/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-05-30 16:36:16.000000 somacore-1.0.3/python-spec/src/somacore/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-05-30 16:36:16.000000 somacore-1.0.3/python-spec/src/somacore/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19708 2023-05-30 16:36:16.000000 somacore-1.0.3/python-spec/src/somacore/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:36:36.585210 somacore-1.0.3/python-spec/src/somacore/ephemeral/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-30 16:36:16.000000 somacore-1.0.3/python-spec/src/somacore/ephemeral/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-05-30 16:36:16.000000 somacore-1.0.3/python-spec/src/somacore/ephemeral/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-05-30 16:36:16.000000 somacore-1.0.3/python-spec/src/somacore/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-05-30 16:36:16.000000 somacore-1.0.3/python-spec/src/somacore/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-05-30 16:36:16.000000 somacore-1.0.3/python-spec/src/somacore/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-30 16:36:16.000000 somacore-1.0.3/python-spec/src/somacore/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:36:36.585210 somacore-1.0.3/python-spec/src/somacore/query/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-30 16:36:16.000000 somacore-1.0.3/python-spec/src/somacore/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-30 16:36:16.000000 somacore-1.0.3/python-spec/src/somacore/query/_eager_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-05-30 16:36:16.000000 somacore-1.0.3/python-spec/src/somacore/query/_fast_csr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-05-30 16:36:16.000000 somacore-1.0.3/python-spec/src/somacore/query/axis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18096 2023-05-30 16:36:16.000000 somacore-1.0.3/python-spec/src/somacore/query/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-05-30 16:36:16.000000 somacore-1.0.3/python-spec/src/somacore/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:36:36.585210 somacore-1.0.3/python-spec/src/somacore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-30 16:36:36.000000 somacore-1.0.3/python-spec/src/somacore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 16:36:36.585210 somacore-1.0.3/setup.cfg
```

### Comparing `somacore-1.0.2/LICENSE` & `somacore-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `somacore-1.0.2/PKG-INFO` & `somacore-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: somacore
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python-language API specification and base utilities for implementation of the SOMA system.
 Project-URL: repository, https://github.com/single-cell-data/SOMA.git
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `somacore-1.0.2/pyproject.toml` & `somacore-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `somacore-1.0.2/python-spec/README.md` & `somacore-1.0.3/python-spec/README.md`

 * *Files identical despite different names*

### Comparing `somacore-1.0.2/python-spec/src/somacore/__init__.py` & `somacore-1.0.3/python-spec/src/somacore/__init__.py`

 * *Files identical despite different names*

### Comparing `somacore-1.0.2/python-spec/src/somacore/_mixin.py` & `somacore-1.0.3/python-spec/src/somacore/_mixin.py`

 * *Files identical despite different names*

### Comparing `somacore-1.0.2/python-spec/src/somacore/collection.py` & `somacore-1.0.3/python-spec/src/somacore/collection.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 ):
     """A generic string-keyed collection of :class:`base.SOMAObject`s.
 
     The generic type specifies what type the Collection may contain. At its
     most generic, a Collection may contain any SOMA object, but a subclass
     may specify that it is a Collection of a specific type of SOMA object.
 
-    Lifecycle: experimental
+    Lifecycle: maturing
     """
 
     __slots__ = ()
 
     @classmethod
     @abc.abstractmethod
     def create(
@@ -39,15 +39,15 @@
     ) -> Self:
         """Creates a new collection of this type at the given URI.
 
         Args:
             uri: The URI where the collection will be created.
         Returns:
             The newly created collection, opened for writing.
-        Lifecycle: experimental
+        Lifecycle: maturing
         """
         raise NotImplementedError()
 
     # Overloads to allow type inference to work when doing:
     #
     #     some_coll.add_new_collection("key")  # -> Collection
     # and
@@ -131,15 +131,15 @@
                 If not provided,
             platform_config: Platform-specific configuration options used
                 when creating the child.
 
         Returns:
             The newly created collection, opened for writing.
 
-        Lifecycle: experimental
+        Lifecycle: maturing
         """
         raise NotImplementedError()
 
     @abc.abstractmethod
     def add_new_dataframe(
         self,
         key: str,
@@ -153,15 +153,15 @@
 
         Parameters are as in :meth:`data.DataFrame.create`.
         See :meth:`add_new_collection` for details about child URIs.
 
         Returns:
             The newly created DataFrame, opened for writing.
 
-        Lifecycle: experimental
+        Lifecycle: maturing
         """
         raise NotImplementedError()
 
     @abc.abstractmethod
     def add_new_dense_ndarray(
         self,
         key: str,
@@ -175,15 +175,15 @@
 
         Parameters are as in :meth:`data.DenseNDArray.create`.
         See :meth:`add_new_collection` for details about child URIs.
 
         Returns:
             The newly created dense NDArray, opened for writing.
 
-        Lifecycle: experimental
+        Lifecycle: maturing
         """
         raise NotImplementedError()
 
     @abc.abstractmethod
     def add_new_sparse_ndarray(
         self,
         key: str,
@@ -197,15 +197,15 @@
 
         Parameters are as in :meth:`data.SparseNDArray.create`.
         See :meth:`add_new_collection` for details about child creation.
 
         Returns:
             The newly created sparse NDArray, opened for writing.
 
-        Lifecycle: experimental
+        Lifecycle: maturing
         """
         raise NotImplementedError()
 
     def __setitem__(self, key: str, value: _Elem) -> None:
         """Sets an entry into this collection. See :meth:`set` for details."""
         self.set(key, value)
 
@@ -238,20 +238,20 @@
                 If ``True``, will always use a relative URI. If the new child
                 does not share a relative URI base, or use of relative URIs
                 is not possible at all, the collection should raise an error.
                 If ``False``, will always use an absolute URI.
 
         Returns: ``self``, to enable method chaining.
 
-        Lifecycle: experimental
+        Lifecycle: maturing
         """
         raise NotImplementedError()
 
 
 class Collection(BaseCollection[_Elem]):
     """SOMA Collection imposing no semantics on the contained values.
 
-    Lifecycle: experimental
+    Lifecycle: maturing
     """
 
     soma_type: Final = "SOMACollection"  # type: ignore[misc]
     __slots__ = ()
```

### Comparing `somacore-1.0.2/python-spec/src/somacore/data.py` & `somacore-1.0.3/python-spec/src/somacore/data.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 _RO_AUTO = options.ResultOrder.AUTO
 
 
 class DataFrame(base.SOMAObject, metaclass=abc.ABCMeta):
     """A multi-column table with a user-defined schema.
 
-    Lifecycle: experimental
+    Lifecycle: maturing
     """
 
     __slots__ = ()
     soma_type: Final = "SOMADataFrame"  # type: ignore[misc]
 
     # Lifecycle
 
@@ -83,15 +83,15 @@
                 dimension, the corresponding index-column domain will use
                 the minimum and maximum possible values for the column's
                 datatype.  This makes a dataframe growable.
 
         Returns:
             The newly created dataframe, opened for writing.
 
-        Lifecycle: experimental
+        Lifecycle: maturing
         """
         raise NotImplementedError()
 
     # Data operations
 
     @abc.abstractmethod
     def read(
@@ -151,15 +151,15 @@
           all indices up to and including the value, and all indices
           starting from and including the value.
         - Negative values in indices and slices are treated as raw domain values
           and not as indices relative to the end, unlike traditional Python
           sequence indexing. For instance, ``slice(-10, 3)`` indicates the range
           from −10 to 3 on the given dimension.
 
-        Lifecycle: experimental
+        Lifecycle: maturing
         """
         raise NotImplementedError()
 
     @abc.abstractmethod
     def write(
         self,
         values: Union[pa.RecordBatch, pa.Table],
@@ -174,47 +174,47 @@
         Args:
             values: An Arrow table containing all columns, including
                 the index columns. The schema for the values must match
                 the schema for the ``DataFrame``.
 
         Returns: ``self``, to enable method chaining.
 
-        Lifecycle: experimental
+        Lifecycle: maturing
         """
         raise NotImplementedError()
 
     # Metadata operations
 
     @property
     @abc.abstractmethod
     def schema(self) -> pa.Schema:
         """The schema of the data in this dataframe.
 
-        Lifecycle: experimental
+        Lifecycle: maturing
         """
         raise NotImplementedError()
 
     @property
     @abc.abstractmethod
     def index_column_names(self) -> Tuple[str, ...]:
         """The names of the index (dimension) columns.
 
-        Lifecycle: experimental
+        Lifecycle: maturing
         """
         raise NotImplementedError()
 
     @property
     @abc.abstractmethod
     def domain(self) -> Tuple[Tuple[Any, Any], ...]:
         """The allowable range of values in each index column.
 
         Returns: a tuple of minimum and maximum values, inclusive,
             storable on each index column of the dataframe.
 
-        Lifecycle: experimental
+        Lifecycle: maturing
         """
         raise NotImplementedError()
 
 
 class NDArray(base.SOMAObject, metaclass=abc.ABCMeta):
     """Common behaviors of N-dimensional arrays of a single primitive type."""
 
@@ -248,58 +248,58 @@
                 (N) in the N-dimensional array.
 
                 For sparse arrays only, if a slot is None, then the maximum
                 possible int64 will be used, making a sparse array growable.
 
         Returns: The newly created array, opened for writing.
 
-        Lifecycle: experimental
+        Lifecycle: maturing
         """
         raise NotImplementedError()
 
     # Metadata operations
 
     @property
     @abc.abstractmethod
     def shape(self) -> Tuple[int, ...]:
         """The maximum capacity (domain) of each dimension of this array.
 
-        Lifecycle: experimental
+        Lifecycle: maturing
         """
         raise NotImplementedError()
 
     @property
     def ndim(self) -> int:
         """The number of dimensions in this array.
 
-        Lifecycle: experimental
+        Lifecycle: maturing
         """
         return len(self.shape)
 
     @property
     @abc.abstractmethod
     def schema(self) -> pa.Schema:
         """The schema of the data in this array.
 
-        Lifecycle: experimental
+        Lifecycle: maturing
         """
         raise NotImplementedError()
 
     is_sparse: ClassVar[Literal[True, False]]
     """True if the array is sparse, False if it is dense.
 
-    Lifecycle: experimental
+    Lifecycle: maturing
     """
 
 
 class DenseNDArray(NDArray, metaclass=abc.ABCMeta):
     """
     An N-dimensional array stored densely.
 
-    Lifecycle: experimental
+    Lifecycle: maturing
     """
 
     __slots__ = ()
     soma_type: Final = "SOMADenseNDArray"  # type: ignore[misc]
     is_sparse: Final = False  # type: ignore[misc]
 
     @abc.abstractmethod
@@ -347,15 +347,15 @@
           Slice *steps* may not be used: ``slice(10, 20, 2)`` is invalid.
           ``slice(None)`` places no constraint on the dimension. Half-specified
           slices like ``slice(None, 99)`` and ``slice(5, None)`` specify
           all indices up to and including the value, and all indices
           starting from and including the value.
         - Negative indexing is not supported.
 
-        Lifecycle: experimental
+        Lifecycle: maturing
         """
         raise NotImplementedError()
 
     @abc.abstractmethod
     def write(
         self,
         coords: options.DenseNDCoords,
@@ -371,15 +371,15 @@
         Args:
             coords: A per-dimension tuple of scalars or slices
                 defining the bounds of the subarray to be written.
                 See :meth:`read` for details about indexing.
             values: The values to be written to the subarray.  Must have
                 the same shape as ``coords``, and matching type to the array.
         Returns: ``self``, to enable method chaining.
-        Lifecycle: experimental
+        Lifecycle: maturing
         """
         raise NotImplementedError()
 
 
 SparseArrowData = Union[
     pa.SparseCSCMatrix,
     pa.SparseCSRMatrix,
@@ -388,15 +388,15 @@
 ]
 """Any of the sparse data storages provided by Arrow."""
 
 
 class SparseNDArray(NDArray, metaclass=abc.ABCMeta):
     """A N-dimensional array stored sparsely.
 
-    Lifecycle: experimental
+    Lifecycle: maturing
     """
 
     __slots__ = ()
     soma_type: Final = "SOMASparseNDArray"  # type: ignore[misc]
     is_sparse: Final = True  # type: ignore[misc]
 
     @abc.abstractmethod
@@ -452,15 +452,15 @@
           Slice *steps* may not be used: ``slice(10, 20, 2)`` is invalid.
           ``slice(None)`` places no constraint on the dimension. Half-specified
           slices like ``slice(None, 99)`` and ``slice(5, None)`` specify
           all indices up to and including the value, and all indices
           starting from and including the value.
         - Negative indexing is not supported.
 
-        Lifecycle: experimental
+        Lifecycle: maturing
         """
 
     @abc.abstractmethod
     def write(
         self,
         values: SparseArrowData,
         *,
@@ -478,23 +478,23 @@
                 SparseCSFTensor or dense Tensor.
 
                 Arrow table: a COO table, with columns named ``soma_dim_0``,
                     ..., ``soma_dim_N`` and ``soma_data``.
 
         Returns: ``self``, to enable method chaining.
 
-        Lifecycle: experimental
+        Lifecycle: maturing
         """
         raise NotImplementedError()
 
     @property
     def nnz(self) -> int:
         """The number of values stored in the array, including explicit zeros.
 
-        Lifecycle: experimental
+        Lifecycle: maturing
         """
         raise NotImplementedError()
 
 
 #
 # Read types
 #
@@ -504,43 +504,43 @@
 
 # Sparse reads are returned as an iterable structure:
 
 
 class ReadIter(Iterator[_T], metaclass=abc.ABCMeta):
     """SparseRead result iterator allowing users to flatten the iteration.
 
-    Lifecycle: experimental
+    Lifecycle: maturing
     """
 
     __slots__ = ()
 
     # __iter__ is already implemented as `return self` in Iterator.
     # SOMA implementations must implement __next__.
 
     @abc.abstractmethod
     def concat(self) -> _T:
         """Returns all the requested data in a single operation.
 
         If some data has already been retrieved using ``next``, this will return
         the remaining data, excluding that which as already been returned.
 
-        Lifecycle: experimental
+        Lifecycle: maturing
         """
         raise NotImplementedError()
 
 
 class SparseRead:
     """Intermediate type to choose result format when reading a sparse array.
 
     A query may not be able to return all of these formats. The concrete result
     may raise a ``NotImplementedError`` or may choose to raise a different
     exception (likely a ``TypeError``) containing more specific information
     about why the given format is not supported.
 
-    Lifecycle: experimental
+    Lifecycle: maturing
     """
 
     __slots__ = ()
 
     def coos(self) -> ReadIter[pa.SparseCOOTensor]:
         raise NotImplementedError()
```

### Comparing `somacore-1.0.2/python-spec/src/somacore/ephemeral/collections.py` & `somacore-1.0.3/python-spec/src/somacore/ephemeral/collections.py`

 * *Files identical despite different names*

### Comparing `somacore-1.0.2/python-spec/src/somacore/experiment.py` & `somacore-1.0.3/python-spec/src/somacore/experiment.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     """A collection subtype representing an annotated 2D matrix of measurements.
 
     In single cell biology, this can represent multiple modes of measurement
     across a single collection of cells (i.e., a "multimodal dataset").
     Within an experiment, a set of measurements on a single set of variables
     (i.e., features) is represented as a :class:`~measurement.Measurement`.
 
-    Lifecycle: experimental
+    Lifecycle: maturing
     """
 
     # This class is implemented as a mixin to be used with SOMA classes.
     # For example, a SOMA implementation would look like this:
     #
     #     # This type-ignore comment will always be needed due to limitations
     #     # of type annotations; it is (currently) expected.
@@ -64,15 +64,15 @@
         obs_query: Optional[query.AxisQuery] = None,
         var_query: Optional[query.AxisQuery] = None,
     ) -> "query.ExperimentAxisQuery[Self]":
         """Creates an axis query over this experiment.
 
         See :class:`query.ExperimentAxisQuery` for details on usage.
 
-        Lifecycle: experimental
+        Lifecycle: maturing
         """
         # mypy doesn't quite understand descriptors so it issues a spurious
         # error here.
         return query.ExperimentAxisQuery(  # type: ignore[type-var]
             self,
             measurement_name,
             obs_query=obs_query or query.AxisQuery(),
```

### Comparing `somacore-1.0.2/python-spec/src/somacore/measurement.py` & `somacore-1.0.3/python-spec/src/somacore/measurement.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     in sparse and dense ND arrays.
 
     The observables are inherited from the parent ``Experiment``'s
     ``obs`` dataframe. The ``soma_joinid`` of these observables (``obsid``),
     along with those of the measurement's ``var`` dataframe (``varid``),
     are the indices for all the other matrices stored in the measurement.
 
-    Lifecycle: experimental
+    Lifecycle: maturing
     """
 
     # This class is implemented as a mixin to be used with SOMA classes.
     # For example, a SOMA implementation would look like this:
     #
     #     # This type-ignore comment will always be needed due to limitations
     #     # of type annotations; it is (currently) expected.
```

### Comparing `somacore-1.0.2/python-spec/src/somacore/options.py` & `somacore-1.0.3/python-spec/src/somacore/options.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Enums and other types used as options across methods of many types.
 
 These types are *concrete* and should be used as-is as inputs to the various
 SOMA types that require them, not reimplemented by the implementing package.
 """
 
 import enum
-from typing import Any, Mapping, Optional, Sequence, TypeVar, Union
+from typing import Any, Dict, Mapping, Optional, Sequence, TypeVar, Union
 
 import attrs
 import numpy as np
 import numpy.typing as npt
 import pyarrow as pa
 from typing_extensions import Final, Literal
 
@@ -97,20 +97,28 @@
             return  # None (or 0, which we treat equivalently) is always valid.
         if value < 0:
             raise ValueError(f"If set, '{attr.name}' must be positive")
         if self.count and self.bytes:
             raise ValueError("Either 'count' or 'bytes' may be set, not both")
 
 
-PlatformConfig = Mapping[str, Any]
+PlatformConfig = Union[Dict[str, Mapping[str, Any]], object]
 """Type alias for the ``platform_config`` parameter.
 
 ``platform_config`` allows platform-specific configuration data to be passed
-to individual calls. Keys are the name of a SOMA implementation, each value is
-an implementation-defined configuration structure.
+to individual calls. This is either a ``dict``, or an implementation-specific
+configuration object:
+
+- If a dictionary, the keys to the dictionary are the name of a SOMA
+  implementation, and the value of the dictionary is configuration specific to
+  that implementation.
+- If an implementation-specific object, that implementation will use that object
+  for configuration data; it will be ignored by others.
+
+See the "Per-call configuration" section of the main SOMA specifiction.
 """
 
 
 class ResultOrder(enum.Enum):
     """
     The order results should be returned in.
```

### Comparing `somacore-1.0.2/python-spec/src/somacore/query/_eager_iter.py` & `somacore-1.0.3/python-spec/src/somacore/query/_eager_iter.py`

 * *Files identical despite different names*

### Comparing `somacore-1.0.2/python-spec/src/somacore/query/_fast_csr.py` & `somacore-1.0.3/python-spec/src/somacore/query/_fast_csr.py`

 * *Files identical despite different names*

### Comparing `somacore-1.0.2/python-spec/src/somacore/query/axis.py` & `somacore-1.0.3/python-spec/src/somacore/query/axis.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         AxisQuery(coords=())  # also all data
         AxisQuery(coords=(slice(1,10),))  # 1D, slice
         AxisQuery(coords=([0,1,2]))  # 1D, point indexing using array-like
         AxisQuery(coords=(slice(None), numpy.array([0,88,1001])))  # 2D
         AxisQuery(value_filter="tissue == 'lung'")
         AxisQuery(coords=(slice(1,None),), value_filter="tissue == 'lung'")
 
-    Lifecycle: experimental
+    Lifecycle: maturing
     """
 
     value_filter: Optional[str] = attrs.field(
         default=None,
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
     )
     """A string specifying a SOMA ``value_filter``."""
```

### Comparing `somacore-1.0.2/python-spec/src/somacore/query/query.py` & `somacore-1.0.3/python-spec/src/somacore/query/query.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from . import axis
 
 
 class AxisColumnNames(TypedDict, total=False):
     """
     Specifies column names for experiment axis query read operations.
 
-    Lifecycle: experimental
+    Lifecycle: maturing
     """
 
     obs: Optional[Sequence[str]]
     """obs columns to use. All columns if ``None`` or not present."""
     var: Optional[Sequence[str]]
     """var columns to use. All columns if ``None`` or not present."""
 
@@ -70,15 +70,15 @@
         with ExperimentAxisQuery(...) as query:
             ...
 
     This base query implementation is designed to work against any SOMA
     implementation that fulfills the basic APIs. A SOMA implementation may
     include a custom query implementation optimized for its own use.
 
-    Lifecycle: experimental
+    Lifecycle: maturing
     """
 
     def __init__(
         self,
         experiment: _Exp,
         measurement_name: str,
         *,
@@ -99,15 +99,15 @@
     def obs(
         self, *, column_names: Optional[Sequence[str]] = None
     ) -> data.ReadIter[pa.Table]:
         """Returns ``obs`` as an `Arrow table
         <https://arrow.apache.org/docs/python/generated/pyarrow.Table.html>`_
         iterator.
 
-        Lifecycle: experimental
+        Lifecycle: maturing
         """
         obs_query = self._matrix_axis_query.obs
         return self._obs_df.read(
             obs_query.coords,
             value_filter=obs_query.value_filter,
             column_names=column_names,
         )
@@ -115,90 +115,90 @@
     def var(
         self, *, column_names: Optional[Sequence[str]] = None
     ) -> data.ReadIter[pa.Table]:
         """Returns ``var`` as an `Arrow table
         <https://arrow.apache.org/docs/python/generated/pyarrow.Table.html>`_
         iterator.
 
-        Lifecycle: experimental
+        Lifecycle: maturing
         """
         var_query = self._matrix_axis_query.var
         return self._var_df.read(
             var_query.coords,
             value_filter=var_query.value_filter,
             column_names=column_names,
         )
 
     def obs_joinids(self) -> pa.Array:
         """Returns ``obs`` ``soma_joinids`` as an Arrow array.
 
-        Lifecycle: experimental
+        Lifecycle: maturing
         """
         return self._joinids.obs
 
     def var_joinids(self) -> pa.Array:
         """Returns ``var`` ``soma_joinids`` as an Arrow array.
 
-        Lifecycle: experimental
+        Lifecycle: maturing
         """
         return self._joinids.var
 
     @property
     def n_obs(self) -> int:
         """The number of ``obs`` axis query results.
 
-        Lifecycle: experimental
+        Lifecycle: maturing
         """
         return len(self.obs_joinids())
 
     @property
     def n_vars(self) -> int:
         """The number of ``var`` axis query results.
 
-        Lifecycle: experimental
+        Lifecycle: maturing
         """
         return len(self.var_joinids())
 
     @property
     def indexer(self) -> "AxisIndexer":
         """A ``soma_joinid`` indexer for both ``obs`` and ``var`` axes.
 
-        Lifecycle: experimental
+        Lifecycle: maturing
         """
         return self._indexer
 
     def X(self, layer_name: str) -> data.SparseRead:
         """Returns an ``X`` layer as a sparse read.
 
         Args:
             layer_name: The X layer name to return.
 
-        Lifecycle: experimental
+        Lifecycle: maturing
         """
         try:
             x_layer = self._ms.X[layer_name]
         except KeyError as ke:
             raise KeyError(f"{layer_name} is not present in X") from ke
         if not isinstance(x_layer, data.SparseNDArray):
             raise TypeError("X layers may only be sparse arrays")
 
         self._joinids.preload(self._threadpool)
         return x_layer.read((self._joinids.obs, self._joinids.var))
 
     def obsp(self, layer: str) -> data.SparseRead:
         """Returns an ``obsp`` layer as a sparse read.
 
-        Lifecycle: experimental
+        Lifecycle: maturing
         """
         return self._axisp_inner(_Axis.OBS, layer)
 
     def varp(self, layer: str) -> data.SparseRead:
         """Returns an ``varp`` layer as a sparse read.
 
-        Lifecycle: experimental
+        Lifecycle: maturing
         """
         return self._axisp_inner(_Axis.VAR, layer)
 
     def to_anndata(
         self,
         X_name: str,
         *,
@@ -211,30 +211,30 @@
         Args:
             X_name: The X layer to read and return in the ``X`` slot.
             column_names: The columns in the ``var`` and ``obs`` dataframes
                 to read.
             X_layers: Additional X layers to read and return
                 in the ``layers`` slot.
 
-        Lifecycle: experimental
+        Lifecycle: maturing
         """
         return self._read(
             X_name,
             column_names=column_names or AxisColumnNames(obs=None, var=None),
             X_layers=X_layers,
         ).to_anndata()
 
     # Context management
 
     def close(self) -> None:
         """Releases resources associated with this query.
 
         This method must be idempotent.
 
-        Lifecycle: experimental
+        Lifecycle: maturing
         """
         # Because this may be called during ``__del__`` when we might be getting
         # disassembled, sometimes ``_threadpool_`` is simply missing.
         # Only try to shut it down if it still exists.
         pool = getattr(self, "_threadpool_", None)
         if pool is None:
             return
@@ -522,15 +522,15 @@
 
 
 @attrs.define
 class AxisIndexer:
     """
     Given a query, provides index-building services for obs/var axis.
 
-    Lifecycle: experimental
+    Lifecycle: maturing
     """
 
     query: ExperimentAxisQuery
     _cached_obs: Optional[pd.Index] = None
     _cached_var: Optional[pd.Index] = None
 
     @property
```

### Comparing `somacore-1.0.2/python-spec/src/somacore/types.py` & `somacore-1.0.3/python-spec/src/somacore/types.py`

 * *Files identical despite different names*

### Comparing `somacore-1.0.2/python-spec/src/somacore.egg-info/SOURCES.txt` & `somacore-1.0.3/python-spec/src/somacore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

