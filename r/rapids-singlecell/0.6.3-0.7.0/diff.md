# Comparing `tmp/rapids_singlecell-0.6.3.tar.gz` & `tmp/rapids_singlecell-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapids_singlecell-0.6.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "rapids_singlecell-0.7.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `rapids_singlecell-0.6.3.tar` & `rapids_singlecell-0.7.0.tar`

### file list

```diff
@@ -1,54 +1,58 @@
--rw-r--r--   0        0        0     1070 2023-05-11 09:24:25.229932 rapids_singlecell-0.6.3/LICENSE
--rw-r--r--   0        0        0     5987 2023-05-16 11:43:52.239538 rapids_singlecell-0.6.3/README.md
--rw-r--r--   0        0        0      998 2023-05-11 09:24:26.571232 rapids_singlecell-0.6.3/pyproject.toml
--rwxr-xr-x   0        0        0      132 2023-05-17 23:04:05.157900 rapids_singlecell-0.6.3/rapids_singlecell/__init__.py
--rw-r--r--   0        0        0    13187 2023-05-17 22:08:47.953836 rapids_singlecell-0.6.3/rapids_singlecell/cunnData/__init__.py
--rw-r--r--   0        0        0      334 2023-05-11 09:24:26.629783 rapids_singlecell-0.6.3/rapids_singlecell/cunnData_funcs/__init__.py
--rw-r--r--   0        0        0    36773 2023-05-17 22:13:28.447148 rapids_singlecell-0.6.3/rapids_singlecell/cunnData_funcs/_hvg.py
--rw-r--r--   0        0        0    14574 2023-05-17 22:14:35.602418 rapids_singlecell-0.6.3/rapids_singlecell/cunnData_funcs/_normalize.py
--rw-r--r--   0        0        0     4544 2023-05-17 22:11:30.429802 rapids_singlecell-0.6.3/rapids_singlecell/cunnData_funcs/_pca.py
--rw-r--r--   0        0        0     2783 2023-05-11 09:24:26.706782 rapids_singlecell-0.6.3/rapids_singlecell/cunnData_funcs/_plotting.py
--rw-r--r--   0        0        0     4788 2023-05-16 11:43:52.638546 rapids_singlecell-0.6.3/rapids_singlecell/cunnData_funcs/_regress_out.py
--rw-r--r--   0        0        0     1441 2023-05-17 22:14:46.246296 rapids_singlecell-0.6.3/rapids_singlecell/cunnData_funcs/_scale.py
--rw-r--r--   0        0        0    20285 2023-05-17 22:10:17.988666 rapids_singlecell-0.6.3/rapids_singlecell/cunnData_funcs/_simple.py
--rw-r--r--   0        0        0     3296 2023-05-17 22:15:20.059310 rapids_singlecell-0.6.3/rapids_singlecell/cunnData_funcs/_utils.py
--rw-r--r--   0        0        0       29 2023-04-19 09:06:38.422832 rapids_singlecell-0.6.3/rapids_singlecell/dcg.py
--rw-r--r--   0        0        0       68 2023-04-19 09:06:38.440176 rapids_singlecell-0.6.3/rapids_singlecell/decoupler_gpu/__init__.py
--rw-r--r--   0        0        0     4609 2023-05-11 09:24:27.214977 rapids_singlecell-0.6.3/rapids_singlecell/decoupler_gpu/_method_mlm.py
--rw-r--r--   0        0        0     6349 2023-05-11 09:24:27.233961 rapids_singlecell-0.6.3/rapids_singlecell/decoupler_gpu/_method_wsum.py
--rw-r--r--   0        0        0       27 2023-04-19 09:06:38.463999 rapids_singlecell-0.6.3/rapids_singlecell/gr.py
--rw-r--r--   0        0        0       91 2023-04-19 09:06:38.473434 rapids_singlecell-0.6.3/rapids_singlecell/pl.py
--rw-r--r--   0        0        0       30 2023-05-11 09:24:27.250502 rapids_singlecell-0.6.3/rapids_singlecell/pp.py
--rw-r--r--   0        0        0      340 2023-05-17 22:09:28.847385 rapids_singlecell-0.6.3/rapids_singlecell/scanpy_gpu/__init__.py
--rw-r--r--   0        0        0     5576 2023-05-11 09:24:27.293507 rapids_singlecell-0.6.3/rapids_singlecell/scanpy_gpu/_clustering.py
--rw-r--r--   0        0        0     3422 2023-05-11 09:24:27.312411 rapids_singlecell-0.6.3/rapids_singlecell/scanpy_gpu/_diffmap.py
--rw-r--r--   0        0        0     4040 2023-05-11 09:24:27.331819 rapids_singlecell-0.6.3/rapids_singlecell/scanpy_gpu/_draw_graph.py
--rw-r--r--   0        0        0     5154 2023-05-16 11:43:52.775602 rapids_singlecell-0.6.3/rapids_singlecell/scanpy_gpu/_embedding_density.py
--rw-r--r--   0        0        0    12177 2023-05-11 09:24:27.365884 rapids_singlecell-0.6.3/rapids_singlecell/scanpy_gpu/_harmonpy_gpu.py
--rw-r--r--   0        0        0     1729 2023-05-16 11:43:52.798464 rapids_singlecell-0.6.3/rapids_singlecell/scanpy_gpu/_harmony_integrate.py
--rw-r--r--   0        0        0     2425 2023-05-11 09:24:27.423103 rapids_singlecell-0.6.3/rapids_singlecell/scanpy_gpu/_pymde.py
--rw-r--r--   0        0        0     7928 2023-05-11 09:24:27.442438 rapids_singlecell-0.6.3/rapids_singlecell/scanpy_gpu/_rank_gene_groups.py
--rw-r--r--   0        0        0     3241 2023-05-11 09:24:27.459468 rapids_singlecell-0.6.3/rapids_singlecell/scanpy_gpu/_tsne.py
--rw-r--r--   0        0        0       68 2023-05-11 09:24:27.476729 rapids_singlecell-0.6.3/rapids_singlecell/squidpy_gpu/__init__.py
--rw-r--r--   0        0        0     5949 2023-05-17 22:18:00.040946 rapids_singlecell-0.6.3/rapids_singlecell/squidpy_gpu/_autocorr.py
--rw-r--r--   0        0        0     6440 2023-05-16 11:43:52.844153 rapids_singlecell-0.6.3/rapids_singlecell/squidpy_gpu/_gearysc.py
--rw-r--r--   0        0        0    29505 2023-05-17 22:16:30.013809 rapids_singlecell-0.6.3/rapids_singlecell/squidpy_gpu/_ligrec.py
--rw-r--r--   0        0        0     6298 2023-05-16 11:43:52.894061 rapids_singlecell-0.6.3/rapids_singlecell/squidpy_gpu/_moransi.py
--rw-r--r--   0        0        0     6227 2023-05-17 22:16:29.609203 rapids_singlecell-0.6.3/rapids_singlecell/squidpy_gpu/_utils.py
--rw-r--r--   0        0        0   253384 2023-05-17 15:05:58.944713 rapids_singlecell-0.6.3/rapids_singlecell/tests/_data/dummy.h5ad
--rw-r--r--   0        0        0   602117 2023-05-17 15:57:26.464925 rapids_singlecell-0.6.3/rapids_singlecell/tests/_data/test_data.h5ad
--rw-r--r--   0        0        0    50913 2023-05-17 12:04:20.314112 rapids_singlecell-0.6.3/rapids_singlecell/tests/_scripts/seurat_hvg.csv
--rw-r--r--   0        0        0   397058 2023-05-17 12:04:30.159721 rapids_singlecell-0.6.3/rapids_singlecell/tests/_scripts/seurat_hvg_v3.csv.gz
--rw-r--r--   0        0        0    62865 2023-05-17 12:04:33.776581 rapids_singlecell-0.6.3/rapids_singlecell/tests/_scripts/seurat_hvg_v3_batch.csv
--rw-r--r--   0        0        0     1362 2023-05-17 22:18:37.189568 rapids_singlecell-0.6.3/rapids_singlecell/tests/test_autocorr.py
--rw-r--r--   0        0        0      461 2023-05-17 22:18:37.163485 rapids_singlecell-0.6.3/rapids_singlecell/tests/test_clustering.py
--rw-r--r--   0        0        0      687 2023-05-17 22:18:37.187898 rapids_singlecell-0.6.3/rapids_singlecell/tests/test_emdedding_density.py
--rw-r--r--   0        0        0    10702 2023-05-17 22:18:37.453113 rapids_singlecell-0.6.3/rapids_singlecell/tests/test_hvg.py
--rw-r--r--   0        0        0     6033 2023-05-17 22:18:37.301399 rapids_singlecell-0.6.3/rapids_singlecell/tests/test_ligrec.py
--rw-r--r--   0        0        0     2727 2023-05-17 22:18:37.242297 rapids_singlecell-0.6.3/rapids_singlecell/tests/test_normalization.py
--rw-r--r--   0        0        0     3165 2023-05-17 22:18:37.291646 rapids_singlecell-0.6.3/rapids_singlecell/tests/test_pca.py
--rw-r--r--   0        0        0      532 2023-05-17 22:18:37.177454 rapids_singlecell-0.6.3/rapids_singlecell/tests/test_preprocessing.py
--rw-r--r--   0        0        0     3654 2023-05-17 22:18:37.286524 rapids_singlecell-0.6.3/rapids_singlecell/tests/test_qc_metrics.py
--rw-r--r--   0        0        0     1717 2023-05-17 22:18:37.213145 rapids_singlecell-0.6.3/rapids_singlecell/tests/test_rank_genes_groups_logreg.py
--rw-r--r--   0        0        0       26 2023-04-19 09:06:38.654835 rapids_singlecell-0.6.3/rapids_singlecell/tl.py
--rw-r--r--   0        0        0     6794 1970-01-01 00:00:00.000000 rapids_singlecell-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-30 12:25:00.770346 rapids_singlecell-0.7.0/LICENSE
+-rw-r--r--   0        0        0     5987 2023-05-30 12:25:00.770346 rapids_singlecell-0.7.0/README.md
+-rw-r--r--   0        0        0      998 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/pyproject.toml
+-rwxr-xr-x   0        0        0      132 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/__init__.py
+-rw-r--r--   0        0        0    25027 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/cunnData/__init__.py
+-rw-r--r--   0        0        0      334 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/cunnData_funcs/__init__.py
+-rw-r--r--   0        0        0    36773 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/cunnData_funcs/_hvg.py
+-rw-r--r--   0        0        0    14581 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/cunnData_funcs/_normalize.py
+-rw-r--r--   0        0        0     4544 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/cunnData_funcs/_pca.py
+-rw-r--r--   0        0        0     2783 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/cunnData_funcs/_plotting.py
+-rw-r--r--   0        0        0     4795 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/cunnData_funcs/_regress_out.py
+-rw-r--r--   0        0        0     1441 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/cunnData_funcs/_scale.py
+-rw-r--r--   0        0        0    18267 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/cunnData_funcs/_simple.py
+-rw-r--r--   0        0        0     3351 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/cunnData_funcs/_utils.py
+-rw-r--r--   0        0        0       29 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/dcg.py
+-rw-r--r--   0        0        0       68 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/decoupler_gpu/__init__.py
+-rw-r--r--   0        0        0     4609 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/decoupler_gpu/_method_mlm.py
+-rw-r--r--   0        0        0     6349 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/decoupler_gpu/_method_wsum.py
+-rw-r--r--   0        0        0       27 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/gr.py
+-rw-r--r--   0        0        0       91 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/pl.py
+-rw-r--r--   0        0        0       30 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/pp.py
+-rw-r--r--   0        0        0      340 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/scanpy_gpu/__init__.py
+-rw-r--r--   0        0        0     5576 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/scanpy_gpu/_clustering.py
+-rw-r--r--   0        0        0     3429 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/scanpy_gpu/_diffmap.py
+-rw-r--r--   0        0        0     4040 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/scanpy_gpu/_draw_graph.py
+-rw-r--r--   0        0        0     5154 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/scanpy_gpu/_embedding_density.py
+-rw-r--r--   0        0        0    12177 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/scanpy_gpu/_harmonpy_gpu.py
+-rw-r--r--   0        0        0     1729 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/scanpy_gpu/_harmony_integrate.py
+-rw-r--r--   0        0        0     2425 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/scanpy_gpu/_pymde.py
+-rw-r--r--   0        0        0     7928 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/scanpy_gpu/_rank_gene_groups.py
+-rw-r--r--   0        0        0     3241 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/scanpy_gpu/_tsne.py
+-rw-r--r--   0        0        0       68 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/squidpy_gpu/__init__.py
+-rw-r--r--   0        0        0     6012 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/squidpy_gpu/_autocorr.py
+-rw-r--r--   0        0        0     6467 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/squidpy_gpu/_gearysc.py
+-rw-r--r--   0        0        0    29539 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/squidpy_gpu/_ligrec.py
+-rw-r--r--   0        0        0     6325 2023-05-30 12:25:01.054366 rapids_singlecell-0.7.0/rapids_singlecell/squidpy_gpu/_moransi.py
+-rw-r--r--   0        0        0     6227 2023-05-30 12:25:01.054366 rapids_singlecell-0.7.0/rapids_singlecell/squidpy_gpu/_utils.py
+-rw-r--r--   0        0        0      571 2023-05-30 12:25:01.054366 rapids_singlecell-0.7.0/rapids_singlecell/tests/README.md
+-rw-r--r--   0        0        0   253384 2023-05-30 12:25:01.054366 rapids_singlecell-0.7.0/rapids_singlecell/tests/_data/dummy.h5ad
+-rw-r--r--   0        0        0   106788 2023-05-30 12:25:01.054366 rapids_singlecell-0.7.0/rapids_singlecell/tests/_data/paul15_means.pickle
+-rw-r--r--   0        0        0   602117 2023-05-30 12:25:01.058367 rapids_singlecell-0.7.0/rapids_singlecell/tests/_data/test_data.h5ad
+-rw-r--r--   0        0        0    50913 2023-05-30 12:25:01.058367 rapids_singlecell-0.7.0/rapids_singlecell/tests/_scripts/seurat_hvg.csv
+-rw-r--r--   0        0        0   397058 2023-05-30 12:25:01.058367 rapids_singlecell-0.7.0/rapids_singlecell/tests/_scripts/seurat_hvg_v3.csv.gz
+-rw-r--r--   0        0        0    62865 2023-05-30 12:25:01.058367 rapids_singlecell-0.7.0/rapids_singlecell/tests/_scripts/seurat_hvg_v3_batch.csv
+-rw-r--r--   0        0        0     1362 2023-05-30 12:25:01.058367 rapids_singlecell-0.7.0/rapids_singlecell/tests/test_autocorr.py
+-rw-r--r--   0        0        0      461 2023-05-30 12:25:01.058367 rapids_singlecell-0.7.0/rapids_singlecell/tests/test_clustering.py
+-rw-r--r--   0        0        0    10341 2023-05-30 12:25:01.058367 rapids_singlecell-0.7.0/rapids_singlecell/tests/test_cunndata.py
+-rw-r--r--   0        0        0     2246 2023-05-30 12:25:01.058367 rapids_singlecell-0.7.0/rapids_singlecell/tests/test_decoupler.py
+-rw-r--r--   0        0        0      687 2023-05-30 12:25:01.058367 rapids_singlecell-0.7.0/rapids_singlecell/tests/test_emdedding_density.py
+-rw-r--r--   0        0        0    10622 2023-05-30 12:25:01.058367 rapids_singlecell-0.7.0/rapids_singlecell/tests/test_hvg.py
+-rw-r--r--   0        0        0    12995 2023-05-30 12:25:01.058367 rapids_singlecell-0.7.0/rapids_singlecell/tests/test_ligrec.py
+-rw-r--r--   0        0        0     2727 2023-05-30 12:25:01.058367 rapids_singlecell-0.7.0/rapids_singlecell/tests/test_normalization.py
+-rw-r--r--   0        0        0     3165 2023-05-30 12:25:01.058367 rapids_singlecell-0.7.0/rapids_singlecell/tests/test_pca.py
+-rw-r--r--   0        0        0      532 2023-05-30 12:25:01.058367 rapids_singlecell-0.7.0/rapids_singlecell/tests/test_preprocessing.py
+-rw-r--r--   0        0        0     3654 2023-05-30 12:25:01.058367 rapids_singlecell-0.7.0/rapids_singlecell/tests/test_qc_metrics.py
+-rw-r--r--   0        0        0     1717 2023-05-30 12:25:01.058367 rapids_singlecell-0.7.0/rapids_singlecell/tests/test_rank_genes_groups_logreg.py
+-rw-r--r--   0        0        0       26 2023-05-30 12:25:01.058367 rapids_singlecell-0.7.0/rapids_singlecell/tl.py
+-rw-r--r--   0        0        0     6794 1970-01-01 00:00:00.000000 rapids_singlecell-0.7.0/PKG-INFO
```

### Comparing `rapids_singlecell-0.6.3/LICENSE` & `rapids_singlecell-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.3/README.md` & `rapids_singlecell-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.3/pyproject.toml` & `rapids_singlecell-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.3/rapids_singlecell/cunnData_funcs/_hvg.py` & `rapids_singlecell-0.7.0/rapids_singlecell/cunnData_funcs/_hvg.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.3/rapids_singlecell/cunnData_funcs/_normalize.py` & `rapids_singlecell-0.7.0/rapids_singlecell/cunnData_funcs/_normalize.py`

 * *Files 0% similar despite different names*

```diff
@@ -333,15 +333,15 @@
     if clip < 0:
         raise ValueError("Pearson residuals require `clip>=0` or `clip=None`.")
     theta = cp.array([1 / theta], dtype=cp.float32)
     clip = cp.array([clip], dtype=cp.float32)
     sums_cells = cp.zeros(X.shape[0], dtype=cp.float32)
     sums_genes = cp.zeros(X.shape[1], dtype=cp.float32)
 
-    if cp.sparse.issparse(X):
+    if cpx.scipy.sparse.issparse(X):
         residuals = cp.zeros(X.shape, dtype=cp.float32)
         if cpx.scipy.sparse.isspmatrix_csc(X):
             block = (8,)
             grid = (int(math.ceil(X.shape[1] / block[0])),)
             _sparse_kernel_sum_csc(
                 grid,
                 block,
```

### Comparing `rapids_singlecell-0.6.3/rapids_singlecell/cunnData_funcs/_pca.py` & `rapids_singlecell-0.7.0/rapids_singlecell/cunnData_funcs/_pca.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.3/rapids_singlecell/cunnData_funcs/_plotting.py` & `rapids_singlecell-0.7.0/rapids_singlecell/cunnData_funcs/_plotting.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.3/rapids_singlecell/cunnData_funcs/_regress_out.py` & `rapids_singlecell-0.7.0/rapids_singlecell/cunnData_funcs/_regress_out.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
     y : cupy.sparse.spmatrix of shape (n_cells,)
         Sparse matrix containing a single column of the cellxgene matrix
     Returns
     -------
     dense_mat : cupy.ndarray of shape (n_cells,)
         Adjusted column
     """
-    if cp.sparse.issparse(y):
+    if cpx.scipy.sparse.issparse(y):
         y = y.todense()
 
     lr = LinearRegression(fit_intercept=False, output_type="cupy")
     lr.fit(X, y, convert_dtype=True)
     return y.reshape(
         y.shape[0],
     ) - lr.predict(
```

### Comparing `rapids_singlecell-0.6.3/rapids_singlecell/cunnData_funcs/_scale.py` & `rapids_singlecell-0.7.0/rapids_singlecell/cunnData_funcs/_scale.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.3/rapids_singlecell/cunnData_funcs/_simple.py` & `rapids_singlecell-0.7.0/rapids_singlecell/cunnData_funcs/_simple.py`

 * *Files 10% similar despite different names*

```diff
@@ -215,15 +215,15 @@
     """
 
     X = cudata.X
     sums_cells = cp.zeros(X.shape[0], dtype=cp.float32)
     sums_genes = cp.zeros(X.shape[1], dtype=cp.float32)
     cell_ex = cp.zeros(X.shape[0], dtype=cp.int32)
     gene_ex = cp.zeros(X.shape[1], dtype=cp.int32)
-    if cp.sparse.issparse(X):
+    if cpx.scipy.sparse.issparse(X):
         if cpx.scipy.sparse.isspmatrix_csr(X):
             block = (32,)
             grid = (int(math.ceil(X.shape[0] / block[0])),)
             _sparse_qc_kernel_csr(
                 grid,
                 block,
                 (
@@ -288,15 +288,15 @@
 
     if qc_vars:
         if type(qc_vars) is str:
             qc_vars = [qc_vars]
         for qc_var in qc_vars:
             sums_cells_sub = cp.zeros(X.shape[0], dtype=cp.float32)
             mask = cp.array(cudata.var[qc_var], dtype=cp.bool_)
-            if cp.sparse.issparse(X):
+            if cpx.scipy.sparse.issparse(X):
                 if cpx.scipy.sparse.isspmatrix_csr(X):
                     block = (32,)
                     grid = (int(math.ceil(X.shape[0] / block[0])),)
                     _sparse_qc_kernel_csr_sub(
                         grid,
                         block,
                         (X.indptr, X.indices, X.data, sums_cells_sub, mask, X.shape[0]),
@@ -415,27 +415,16 @@
         elif max_count is not None:
             thr = np.where(cudata.var[qc_var] <= max_count)[0]
 
         if verbose:
             print(
                 f"filtered out {cudata.var.shape[0]-thr.shape[0]} genes based on {qc_var}"
             )
-        cudata.X = cudata.X.tocsr()
-        cudata.X = cudata.X[:, thr]
-        cudata.X = cudata.X.tocsr()
-        cudata.var = cudata.var.iloc[cp.asnumpy(thr)]
-        if cudata.layers:
-            for key, matrix in cudata.layers.items():
-                cudata.layers[key] = matrix[:, thr]
-        if cudata.varm:
-            for key, matrix in cudata.varm.items():
-                if isinstance(matrix, pd.DataFrame):
-                    cudata.varm[key] = matrix.iloc[thr, :]
-                else:
-                    cudata.varm[key] = matrix[thr, :]
+
+        cudata._inplace_subset_var(thr)
 
     elif qc_var in [
         "n_cells_by_counts",
         "total_counts",
         "mean_counts",
         "pct_dropout_by_counts",
     ]:
@@ -452,26 +441,16 @@
         elif max_count is not None:
             thr = np.where(cudata.var[qc_var] <= max_count)[0]
 
         if verbose:
             print(
                 f"filtered out {cudata.var.shape[0]-thr.shape[0]} genes based on {qc_var}"
             )
-        cudata.X = cudata.X[:, thr]
-        if cudata.layers:
-            for key, matrix in cudata.layers.items():
-                cudata.layers[key] = matrix[:, thr]
-        if cudata.varm:
-            for key, matrix in cudata.varm.items():
-                if isinstance(matrix, pd.DataFrame):
-                    cudata.varm[key] = matrix.iloc[thr, :]
-                else:
-                    cudata.varm[key] = matrix[thr, :]
 
-        cudata.var = cudata.var.iloc[cp.asnumpy(thr)]
+        cudata._inplace_subset_var(thr)
     else:
         print(f"please check qc_var")
 
 
 def filter_cells(
     cudata: cunnData,
     qc_var: str,
@@ -513,23 +492,15 @@
             inter = np.where(cudata.obs[qc_var] > min_count)[0]
         elif max_count is not None:
             inter = np.where(cudata.obs[qc_var] < max_count)[0]
         else:
             print(f"Please specify a cutoff to filter against")
         if verbose:
             print(f"filtered out {cudata.obs.shape[0]-inter.shape[0]} cells")
-        cudata.X = cudata.X[inter, :]
-        cudata.obs = cudata.obs.iloc[inter]
-        cudata._update_shape()
-        if cudata.layers:
-            for key, matrix in cudata.layers.items():
-                cudata.layers[key] = matrix[inter, :]
-        if cudata.obsm:
-            for key, matrix in cudata.obsm.items():
-                cudata.obsm[key] = matrix[inter, :]
+        cudata._inplace_subset_obs(inter)
     elif qc_var in ["n_genes_by_counts", "total_counts"]:
         print(
             f"Running `calculate_qc_metrics` for 'n_cells_by_counts' or 'total_counts'"
         )
         calculate_qc_metrics(cudata, log1p=False)
         inter = np.array
         if min_count is not None and max_count is not None:
@@ -540,22 +511,15 @@
             inter = np.where(cudata.obs[qc_var] > min_count)[0]
         elif max_count is not None:
             inter = np.where(cudata.obs[qc_var] < max_count)[0]
         else:
             print(f"Please specify a cutoff to filter against")
         if verbose:
             print(f"filtered out {cudata.obs.shape[0]-inter.shape[0]} cells")
-        cudata.X = cudata.X[inter, :]
-        cudata.obs = cudata.obs.iloc[inter]
-        if cudata.layers:
-            for key, matrix in cudata.layers.items():
-                cudata.layers[key] = matrix[inter, :]
-        if cudata.obsm:
-            for key, matrix in cudata.obsm.items():
-                cudata.obsm[key] = matrix[inter, :]
+        cudata._inplace_subset_obs(inter)
     else:
         print(f"Please check qc_var.")
 
 
 def filter_highly_variable(cudata: cunnData) -> None:
     """
     Filters the :class:`~rapids_singlecell.cunnData.cunnData` object for highly_variable genes. Run highly_varible_genes first.
@@ -563,20 +527,10 @@
     Returns
     -------
         updates :class:`~rapids_singlecell.cunnData.cunnData` object to only contain highly variable genes.
 
     """
     if "highly_variable" in cudata.var.keys():
         thr = np.where(cudata.var["highly_variable"] == True)[0]
-        cudata.X = cudata.X[:, thr]
-        cudata.var = cudata.var.iloc[thr]
-        if cudata.layers:
-            for key, matrix in cudata.layers.items():
-                cudata.layers[key] = matrix[:, thr]
-        if cudata.varm:
-            for key, matrix in cudata.varm.items():
-                if isinstance(matrix, pd.DataFrame):
-                    cudata.varm[key] = matrix.iloc[thr, :]
-                else:
-                    cudata.varm[key] = matrix[thr, :]
+        cudata._inplace_subset_var(thr)
     else:
         print(f"Please calculate highly variable genes first")
```

### Comparing `rapids_singlecell-0.6.3/rapids_singlecell/cunnData_funcs/_utils.py` & `rapids_singlecell-0.7.0/rapids_singlecell/cunnData_funcs/_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import cupy as cp
-from cupy.sparse import issparse
+import cupyx as cpx
+from cupyx.scipy.sparse import issparse
 import math
 
 _get_mean_var_major = cp.RawKernel(
     r"""
     extern "C" __global__
     void caluclate_meanvar_major(const int *indptr,const int *index,const float *data,
                         double* means,double* vars,
@@ -70,28 +71,28 @@
 
     var = (var - mean**2) * (major / (major - 1))
     return mean, var
 
 
 def _get_mean_var(X, axis=0):
     if axis == 0:
-        if cp.sparse.isspmatrix_csr(X):
+        if cpx.scipy.sparse.isspmatrix_csr(X):
             major = X.shape[0]
             minor = X.shape[1]
             mean, var = _mean_var_major(X, major, minor)
-        elif cp.sparse.isspmatrix_csc(X):
+        elif cpx.scipy.sparse.isspmatrix_csc(X):
             major = X.shape[1]
             minor = X.shape[0]
             mean, var = _mean_var_minor(X, major, minor)
     elif axis == 1:
-        if cp.sparse.isspmatrix_csr(X):
+        if cpx.scipy.sparse.isspmatrix_csr(X):
             major = X.shape[0]
             minor = X.shape[1]
             mean, var = _mean_var_minor(X, major, minor)
-        elif cp.sparse.isspmatrix_csc(X):
+        elif cpx.scipy.sparse.isspmatrix_csc(X):
             major = X.shape[1]
             minor = X.shape[0]
             mean, var = _mean_var_major(X, major, minor)
     return mean, var
 
 
 def _check_nonnegative_integers(X):
```

### Comparing `rapids_singlecell-0.6.3/rapids_singlecell/decoupler_gpu/_method_mlm.py` & `rapids_singlecell-0.7.0/rapids_singlecell/decoupler_gpu/_method_mlm.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.3/rapids_singlecell/decoupler_gpu/_method_wsum.py` & `rapids_singlecell-0.7.0/rapids_singlecell/decoupler_gpu/_method_wsum.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.3/rapids_singlecell/scanpy_gpu/_clustering.py` & `rapids_singlecell-0.7.0/rapids_singlecell/scanpy_gpu/_clustering.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.3/rapids_singlecell/scanpy_gpu/_diffmap.py` & `rapids_singlecell-0.7.0/rapids_singlecell/scanpy_gpu/_diffmap.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     """
 
     if neighbors_key:
         connectivities = adata.obsp[neighbors_key + "_connectivities"]
     else:
         connectivities = adata.obsp["connectivities"]
     if issparse(connectivities):
-        W = cp.sparse.csr_matrix(connectivities, dtype=cp.float32)
+        W = cpx.scipy.sparse.csr_matrix(connectivities, dtype=cp.float32)
     else:
         W = cp.asarray(connectivities)
     if density_normalize:
         # q[i] is an estimate for the sampling density at point i
         # it's also the degree of the underlying graph
         q = cp.asarray(W.sum(axis=0))
         if not cpx.scipy.sparse.issparse(W):
```

### Comparing `rapids_singlecell-0.6.3/rapids_singlecell/scanpy_gpu/_draw_graph.py` & `rapids_singlecell-0.7.0/rapids_singlecell/scanpy_gpu/_draw_graph.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.3/rapids_singlecell/scanpy_gpu/_embedding_density.py` & `rapids_singlecell-0.7.0/rapids_singlecell/scanpy_gpu/_embedding_density.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.3/rapids_singlecell/scanpy_gpu/_harmonpy_gpu.py` & `rapids_singlecell-0.7.0/rapids_singlecell/scanpy_gpu/_harmonpy_gpu.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.3/rapids_singlecell/scanpy_gpu/_harmony_integrate.py` & `rapids_singlecell-0.7.0/rapids_singlecell/scanpy_gpu/_harmony_integrate.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.3/rapids_singlecell/scanpy_gpu/_pymde.py` & `rapids_singlecell-0.7.0/rapids_singlecell/scanpy_gpu/_pymde.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.3/rapids_singlecell/scanpy_gpu/_rank_gene_groups.py` & `rapids_singlecell-0.7.0/rapids_singlecell/scanpy_gpu/_rank_gene_groups.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.3/rapids_singlecell/scanpy_gpu/_tsne.py` & `rapids_singlecell-0.7.0/rapids_singlecell/scanpy_gpu/_tsne.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.3/rapids_singlecell/squidpy_gpu/_autocorr.py` & `rapids_singlecell-0.7.0/rapids_singlecell/squidpy_gpu/_autocorr.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     Literal,  # < 3.8
     Sequence,
     Union,
     Optional,
 )
 from scipy import sparse
 import cupy as cp
+import cupyx as cpx
 from ._moransi import _morans_I_cupy
 from ._gearysc import _gearys_C_cupy
 from ._utils import _p_value_calc
 from statsmodels.stats.multitest import multipletests
 
 
 def spatial_autocorr(
@@ -93,28 +94,30 @@
     else:
         if layer:
             vals = adata[:, genes].layers["layer"]
         else:
             vals = adata[:, genes].X
     # create Adj-Matrix
     adj_matrix = adata.obsp[connectivity_key]
-    adj_matrix_cupy = cp.sparse.csr_matrix(adj_matrix, dtype=cp.float32)
+    adj_matrix_cupy = cpx.scipy.sparse.csr_matrix(adj_matrix, dtype=cp.float32)
 
     if transformation:  # row-normalize
         row_sums = adj_matrix_cupy.sum(axis=1).reshape(-1, 1)
         non_zero_rows = row_sums != 0
         row_sums[non_zero_rows] = 1.0 / row_sums[non_zero_rows]
-        adj_matrix_cupy = adj_matrix_cupy.multiply(cp.sparse.csr_matrix(row_sums))
+        adj_matrix_cupy = adj_matrix_cupy.multiply(
+            cpx.scipy.sparse.csr_matrix(row_sums)
+        )
 
     params = {"two_tailed": two_tailed}
 
     # check sparse:
     if use_sparse:
         vals = sparse.csr_matrix(vals)
-        data = cp.sparse.csr_matrix(vals, dtype=cp.float32)
+        data = cpx.scipy.sparse.csr_matrix(vals, dtype=cp.float32)
     else:
         if sparse.issparse(vals):
             vals = vals.toarray()
         data = cp.array(vals, dtype=cp.float32)
     # Run Spartial Autocorr
     if mode == "moran":
         score, score_perms = _morans_I_cupy(
```

### Comparing `rapids_singlecell-0.6.3/rapids_singlecell/squidpy_gpu/_gearysc.py` & `rapids_singlecell-0.7.0/rapids_singlecell/squidpy_gpu/_gearysc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import cupy as cp
+import cupyx as cpx
 import math
 
 
 kernel_gearys_C_num_dense = r"""
 extern "C" __global__ void gearys_C_num_dense(const float* data,
 const int* adj_matrix_row_ptr, const int* adj_matrix_col_ind, const float* adj_matrix_data,
 float* num, int n_samples, int n_features) {
@@ -163,13 +164,13 @@
             cp.cuda.Stream.null.synchronize()
     else:
         gearys_C_permutations = None
     return gearys_C, gearys_C_permutations
 
 
 def _gearys_C_cupy(data, adj_matrix_cupy, n_permutations=100):
-    if cp.sparse.isspmatrix_csr(data):
+    if cpx.scipy.sparse.isspmatrix_csr(data):
         return _gearys_C_cupy_sparse(data, adj_matrix_cupy, n_permutations)
     elif isinstance(data, cp.ndarray):
         return _gearys_C_cupy_dense(data, adj_matrix_cupy, n_permutations)
     else:
         raise ValueError("Datatype not supported")
```

### Comparing `rapids_singlecell-0.6.3/rapids_singlecell/squidpy_gpu/_ligrec.py` & `rapids_singlecell-0.7.0/rapids_singlecell/squidpy_gpu/_ligrec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import cupy as cp
 import numpy as np
 import pandas as pd
 from scipy.sparse import csc_matrix, issparse
-from cupy.sparse import issparse as cpissparse
+from cupyx.scipy.sparse import issparse as cpissparse
+import cupyx as cpx
 import math
 from anndata import AnnData
 from itertools import product
 from typing import (
     Union,
     Literal,
     Optional,
@@ -439,15 +440,15 @@
     )
 
     data["clusters"] = cat.rename_categories(cluster_mapper)
     # much faster than applymap (tested on 1M interactions)
     interactions_ = np.vectorize(lambda g: gene_mapper[g])(interactions.values)
 
     if issparse(mat):
-        data_cp = cp.sparse.csr_matrix(mat.tocsr())
+        data_cp = cpx.scipy.sparse.csr_matrix(mat.tocsr())
     else:
         data_cp = cp.array(mat)
 
     # Convert the 'clusters' column to a CuPy array
     clusters = cp.array(data["clusters"].values, dtype=cp.int32)
 
     # Find the unique clusters and the number of clusters
```

### Comparing `rapids_singlecell-0.6.3/rapids_singlecell/squidpy_gpu/_moransi.py` & `rapids_singlecell-0.7.0/rapids_singlecell/squidpy_gpu/_moransi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import cupy as cp
+import cupyx as cpx
 import math
 
 kernel_morans_I_num_dense = r"""
 extern "C" __global__
 void morans_I_num_dense(const float* data_centered, const int* adj_matrix_row_ptr, const int* adj_matrix_col_ind,
 const float* adj_matrix_data, float* num, int n_samples, int n_features) {
     int f = blockIdx.x * blockDim.x + threadIdx.x;
@@ -155,13 +156,13 @@
             morans_I_permutations[p, :] = num_permuted / den
     else:
         morans_I_permutations = None
     return morans_I, morans_I_permutations
 
 
 def _morans_I_cupy(data, adj_matrix_cupy, n_permutations=100):
-    if cp.sparse.isspmatrix_csr(data):
+    if cpx.scipy.sparse.isspmatrix_csr(data):
         return _morans_I_cupy_sparse(data, adj_matrix_cupy, n_permutations)
     elif isinstance(data, cp.ndarray):
         return _morans_I_cupy_dense(data, adj_matrix_cupy, n_permutations)
     else:
         raise ValueError("Datatype not supported")
```

### Comparing `rapids_singlecell-0.6.3/rapids_singlecell/squidpy_gpu/_utils.py` & `rapids_singlecell-0.7.0/rapids_singlecell/squidpy_gpu/_utils.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.3/rapids_singlecell/tests/_data/dummy.h5ad` & `rapids_singlecell-0.7.0/rapids_singlecell/tests/_data/dummy.h5ad`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.3/rapids_singlecell/tests/_data/test_data.h5ad` & `rapids_singlecell-0.7.0/rapids_singlecell/tests/_data/test_data.h5ad`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.3/rapids_singlecell/tests/_scripts/seurat_hvg.csv` & `rapids_singlecell-0.7.0/rapids_singlecell/tests/_scripts/seurat_hvg.csv`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.3/rapids_singlecell/tests/_scripts/seurat_hvg_v3.csv.gz` & `rapids_singlecell-0.7.0/rapids_singlecell/tests/_scripts/seurat_hvg_v3.csv.gz`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.3/rapids_singlecell/tests/_scripts/seurat_hvg_v3_batch.csv` & `rapids_singlecell-0.7.0/rapids_singlecell/tests/_scripts/seurat_hvg_v3_batch.csv`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.3/rapids_singlecell/tests/test_autocorr.py` & `rapids_singlecell-0.7.0/rapids_singlecell/tests/test_autocorr.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.3/rapids_singlecell/tests/test_emdedding_density.py` & `rapids_singlecell-0.7.0/rapids_singlecell/tests/test_emdedding_density.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.3/rapids_singlecell/tests/test_hvg.py` & `rapids_singlecell-0.7.0/rapids_singlecell/tests/test_hvg.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,20 +3,22 @@
 import cupy as cp
 import cupyx as cpx
 import rapids_singlecell as rsc
 from rapids_singlecell.cunnData import cunnData
 import pandas as pd
 import pytest
 
+from pathlib import Path
 
-def test_highly_variable_genes_basic():
-    cudata = cunnData(sc.datasets.blobs())
+FILE = Path(__file__).parent / Path("_scripts/seurat_hvg.csv")
+FILE_V3 = Path(__file__).parent / Path("_scripts/seurat_hvg_v3.csv.gz")
+FILE_V3_BATCH = Path(__file__).parent / Path("_scripts/seurat_hvg_v3_batch.csv")
 
-    rsc.pp.highly_variable_genes(cudata)
 
+def test_highly_variable_genes_basic():
     cudata = cunnData(sc.datasets.blobs())
     np.random.seed(0)
     cudata.obs["batch"] = np.random.binomial(3, 0.5, size=(cudata.n_obs))
     cudata.obs["batch"] = cudata.obs["batch"].astype("category")
     rsc.pp.highly_variable_genes(cudata, batch_key="batch")
     assert "highly_variable_nbatches" in cudata.var.columns
     assert "highly_variable_intersection" in cudata.var.columns
@@ -65,21 +67,14 @@
         "highly_variable_intersection",
         "highly_variable",
     ]
 
     assert np.all(np.isin(colnames, cudata.var.columns))
 
 
-from pathlib import Path
-
-FILE = Path(__file__).parent / Path("_scripts/seurat_hvg.csv")
-FILE_V3 = Path(__file__).parent / Path("_scripts/seurat_hvg_v3.csv.gz")
-FILE_V3_BATCH = Path(__file__).parent / Path("_scripts/seurat_hvg_v3_batch.csv")
-
-
 def test_higly_variable_genes_compare_to_seurat():
     seurat_hvg_info = pd.read_csv(FILE, sep=" ")
 
     pbmc = sc.datasets.pbmc68k_reduced()
     pbmc.X = pbmc.raw.X
     pbmc.var_names_make_unique()
     pbmc = rsc.cunnData.cunnData(pbmc)
@@ -268,15 +263,15 @@
     # more general checks on ranks, hvg flag and residual variance
     _check_pearson_hvg_columns(cudata.var, n_top_genes)
 
 
 @pytest.mark.parametrize("n_top_genes", [100, 200])
 def test_highly_variable_genes_pearson_residuals_batch(n_top_genes):
     adata = sc.datasets.pbmc3k().copy()
-    adata = adata[:1000, :500]
+    adata = adata[:1000, :500].copy()
     np.random.seed(42)
     adata.obs["batch"] = np.random.randint(0, 3, size=adata.shape[0])
     sc.pp.filter_genes(adata, min_cells=1)
     # cleanup var
     del adata.var
 
     cudata = rsc.cunnData.cunnData(adata)
```

### Comparing `rapids_singlecell-0.6.3/rapids_singlecell/tests/test_normalization.py` & `rapids_singlecell-0.7.0/rapids_singlecell/tests/test_normalization.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.3/rapids_singlecell/tests/test_pca.py` & `rapids_singlecell-0.7.0/rapids_singlecell/tests/test_pca.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.3/rapids_singlecell/tests/test_preprocessing.py` & `rapids_singlecell-0.7.0/rapids_singlecell/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.3/rapids_singlecell/tests/test_qc_metrics.py` & `rapids_singlecell-0.7.0/rapids_singlecell/tests/test_qc_metrics.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.3/rapids_singlecell/tests/test_rank_genes_groups_logreg.py` & `rapids_singlecell-0.7.0/rapids_singlecell/tests/test_rank_genes_groups_logreg.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.3/PKG-INFO` & `rapids_singlecell-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapids_singlecell
-Version: 0.6.3
+Version: 0.7.0
 Summary: running single cell analysis on Nvidia GPUs
 Author: Severin Dicks
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: anndata>=0.7.4
 Requires-Dist: numpy>=1.17.0
 Requires-Dist: decoupler>=1.3.2
```

