# Comparing `tmp/pyqtorch-0.2.6.tar.gz` & `tmp/pyqtorch-0.2.7.tar.gz`

## Comparing `pyqtorch-0.2.6.tar` & `pyqtorch-0.2.7.tar`

### file list

```diff
@@ -1,82 +1,82 @@
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     3301 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/CONTRIBUTING.md
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/README.md
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/mkdocs.yml
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/publish.sh
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/readthedocs.yml
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/setup.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/.github/workflows/run-tests-and-mypy.yml
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/.ruff_cache/content/21836652c37a637f
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/.ruff_cache/content/2602555962d0fc4c
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/.ruff_cache/content/30645ad5f1f1dcfe
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/.ruff_cache/content/317d2f17a1075099
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/.ruff_cache/content/41d845d0f90a6417
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/.ruff_cache/content/617ac8c861e982f1
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/.ruff_cache/content/68cc7f39a1692629
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/.ruff_cache/content/71de32d0dc4ef210
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/.ruff_cache/content/7ab8961a5fd3e34a
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/.ruff_cache/content/7b50e93d7b401d37
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/.ruff_cache/content/7e9bc91eb0e4bec7
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/.ruff_cache/content/8446b77184378e13
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/.ruff_cache/content/8c22cf14dc3075f3
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/.ruff_cache/content/8f831c3208d022cd
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/.ruff_cache/content/963472f7f566f99d
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/.ruff_cache/content/9b70b475da072d2b
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/.ruff_cache/content/a3b4cbbb65fe8420
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/.ruff_cache/content/aaa2c54c6449792b
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/.ruff_cache/content/af9c8e117f709f43
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/.ruff_cache/content/c73abac16d830acc
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/.ruff_cache/content/ce5cb2c96a07a572
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/.ruff_cache/content/ce5dade58b1ccd69
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/.ruff_cache/content/d49ef2d71d47c091
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/.ruff_cache/content/df86f5c8bc05afc4
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/.ruff_cache/content/e69f22aa2552f985
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/.ruff_cache/content/f6f6f60064e20f97
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/.ruff_cache/content/f78c2e380fc669b7
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/docs/CODE_OF_CONDUCT.md -> ../CODE_OF_CONDUCT.md
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/docs/CONTRIBUTING.md -> ../CONTRIBUTING.md
--rw-r--r--   0        0        0    57645 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/docs/QAOA.ipynb
--rw-r--r--   0        0        0     6493 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/docs/essentials.ipynb
--rw-r--r--   0        0        0   154586 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/docs/fit_function.ipynb
--rw-r--r--   0        0        0    74062 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/docs/getting_started.ipynb
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/docs/index.md
--rw-r--r--   0        0        0    46162 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/docs/deprecated/QAOA.ipynb
--rw-r--r--   0        0        0    19339 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/docs/deprecated/bench.py
--rw-r--r--   0        0        0    74042 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/docs/deprecated/fit_function.ipynb
--rw-r--r--   0        0        0   121176 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/docs/deprecated/ham_evol_comparison.ipynb
--rw-r--r--   0        0        0     6459 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/docs/deprecated/state_evolution.ipynb
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/pyqtorch/__init__.py
--rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/pyqtorch/ansatz.py
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/pyqtorch/embedding.py
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/pyqtorch/matrices.py
--rw-r--r--   0        0        0     6255 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/pyqtorch/matrices_sparse.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/pyqtorch/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/pyqtorch/converters/__init__.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/pyqtorch/converters/store_ops.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/pyqtorch/converters/to_qiskit.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/pyqtorch/core/__init__.py
--rw-r--r--   0        0        0    24532 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/pyqtorch/core/batched_operation.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/pyqtorch/core/circuit.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/pyqtorch/core/measurement.py
--rw-r--r--   0        0        0    22213 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/pyqtorch/core/operation.py
--rw-r--r--   0        0        0     5940 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/pyqtorch/core/utils.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/pyqtorch/modules/__init__.py
--rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/pyqtorch/modules/circuit.py
--rw-r--r--   0        0        0     7686 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/pyqtorch/modules/hamevo.py
--rw-r--r--   0        0        0     7730 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/pyqtorch/modules/parametric.py
--rw-r--r--   0        0        0     3417 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/pyqtorch/modules/primitive.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/pyqtorch/modules/utils.py
--rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/tests/conftest.py
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/tests/test_batched_operations.py
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/tests/test_converters.py
--rw-r--r--   0        0        0     5104 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/tests/test_module_hamevo.py
--rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/tests/test_modules.py
--rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/tests/test_operations.py
--rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/tests/test_operations_hamevo.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/LICENSE
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 pyqtorch-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/CONTRIBUTING.md
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/README.md
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/mkdocs.yml
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/readthedocs.yml
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/setup.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.github/workflows/run-tests-and-mypy.yml
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/21836652c37a637f
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/2602555962d0fc4c
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/30645ad5f1f1dcfe
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/317d2f17a1075099
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/41d845d0f90a6417
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/617ac8c861e982f1
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/68cc7f39a1692629
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/71de32d0dc4ef210
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/7ab8961a5fd3e34a
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/7b50e93d7b401d37
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/7e9bc91eb0e4bec7
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/8446b77184378e13
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/8c22cf14dc3075f3
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/8f831c3208d022cd
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/963472f7f566f99d
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/9b70b475da072d2b
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/a3b4cbbb65fe8420
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/aaa2c54c6449792b
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/af9c8e117f709f43
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/c73abac16d830acc
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/ce5cb2c96a07a572
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/ce5dade58b1ccd69
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/d49ef2d71d47c091
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/df86f5c8bc05afc4
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/e69f22aa2552f985
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/f6f6f60064e20f97
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/f78c2e380fc669b7
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/docs/CODE_OF_CONDUCT.md -> ../CODE_OF_CONDUCT.md
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/docs/CONTRIBUTING.md -> ../CONTRIBUTING.md
+-rw-r--r--   0        0        0    57645 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/docs/QAOA.ipynb
+-rw-r--r--   0        0        0     6493 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/docs/essentials.ipynb
+-rw-r--r--   0        0        0   154246 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/docs/fit_function.ipynb
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/docs/index.md
+-rw-r--r--   0        0        0    46162 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/docs/deprecated/QAOA.ipynb
+-rw-r--r--   0        0        0    19339 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/docs/deprecated/bench.py
+-rw-r--r--   0        0        0    74042 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/docs/deprecated/fit_function.ipynb
+-rw-r--r--   0        0        0    74062 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/docs/deprecated/getting_started.ipynb
+-rw-r--r--   0        0        0   121176 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/docs/deprecated/ham_evol_comparison.ipynb
+-rw-r--r--   0        0        0     6459 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/docs/deprecated/state_evolution.ipynb
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/pyqtorch/__init__.py
+-rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/pyqtorch/ansatz.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/pyqtorch/embedding.py
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/pyqtorch/matrices.py
+-rw-r--r--   0        0        0     6255 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/pyqtorch/matrices_sparse.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/pyqtorch/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/pyqtorch/converters/__init__.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/pyqtorch/converters/store_ops.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/pyqtorch/converters/to_qiskit.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/pyqtorch/core/__init__.py
+-rw-r--r--   0        0        0    24532 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/pyqtorch/core/batched_operation.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/pyqtorch/core/circuit.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/pyqtorch/core/measurement.py
+-rw-r--r--   0        0        0    22213 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/pyqtorch/core/operation.py
+-rw-r--r--   0        0        0     5940 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/pyqtorch/core/utils.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/pyqtorch/modules/__init__.py
+-rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/pyqtorch/modules/circuit.py
+-rw-r--r--   0        0        0     7686 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/pyqtorch/modules/hamevo.py
+-rw-r--r--   0        0        0     7730 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/pyqtorch/modules/parametric.py
+-rw-r--r--   0        0        0     3417 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/pyqtorch/modules/primitive.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/pyqtorch/modules/utils.py
+-rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/tests/conftest.py
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/tests/test_batched_operations.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/tests/test_converters.py
+-rw-r--r--   0        0        0     5104 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/tests/test_module_hamevo.py
+-rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/tests/test_modules.py
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/tests/test_notebooks.py
+-rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/tests/test_operations.py
+-rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/tests/test_operations_hamevo.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/LICENSE
+-rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/PKG-INFO
```

### Comparing `pyqtorch-0.2.6/.pre-commit-config.yaml` & `pyqtorch-0.2.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.6/CODE_OF_CONDUCT.md` & `pyqtorch-0.2.7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.6/CONTRIBUTING.md` & `pyqtorch-0.2.7/CONTRIBUTING.md`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 Next, navigate to your new PyQ fork directory and mark the main PyQ repository as the `upstream`:
 
 ```shell
 git remote add upstream https://github.com/pasqal-io/PyQ.git
 ```
 
-## SETUP
+## Setting up your development environment
 
 We recommended to use `hatch` for managing the environments:
 
 To develop within PyQ, use:
 ```shell
 pip install hatch
 hatch -v shell
```

### Comparing `pyqtorch-0.2.6/mkdocs.yml` & `pyqtorch-0.2.7/mkdocs.yml`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 site_name: pyqtorch
 repo_url: "https://github.com/pasqal-io/PyQ"
 repo_name: "PyQ"
 
 nav:
 
-  - Setting up : index.md
-  - Contributing:
+  - Setup : index.md
+  - Contribute:
       - How to Contribute: CONTRIBUTING.md
       - Code of Conduct: CODE_OF_CONDUCT.md
-  - Overview :
+  - Overview:
       - Essentials : essentials.ipynb
   - Tutorials:
-      - Getting started: getting_started.ipynb
       - Fitting a function: fit_function.ipynb
       - QAOA : QAOA.ipynb
 
 
 theme:
   name: material
   features:
```

### Comparing `pyqtorch-0.2.6/.github/workflows/run-tests-and-mypy.yml` & `pyqtorch-0.2.7/.github/workflows/run-tests-and-mypy.yml`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.6/docs/QAOA.ipynb` & `pyqtorch-0.2.7/docs/QAOA.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.6/docs/essentials.ipynb` & `pyqtorch-0.2.7/docs/essentials.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.6/docs/fit_function.ipynb` & `pyqtorch-0.2.7/docs/fit_function.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9885416666666667%*

 * *Differences: {"'cells'": "{1: {'execution_count': None, 'outputs': []}, 2: {'source': {delete: [1, 0]}}, "*

 * *            "insert: [(0, OrderedDict([('attachments', OrderedDict()), ('cell_type', 'markdown'), "*

 * *            "('metadata', OrderedDict()), ('source', ['# Fitting a 1D function'])]))]}"}*

```diff
@@ -1,38 +1,35 @@
 {
     "cells": [
         {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "# Fitting a 1D function"
+            ]
+        },
+        {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": null,
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "/Users/niklas/Library/Application Support/hatch/env/virtual/qucint/6NOL9orC/qucint/lib/python3.9/site-packages/tqdm/auto.py:21: TqdmWarning: IProgress not found. Please update jupyter and ipywidgets. See https://ipywidgets.readthedocs.io/en/stable/user_install.html\n",
-                        "  from .autonotebook import tqdm as notebook_tqdm\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "import matplotlib.pyplot as plt\n",
                 "import torch\n",
                 "\n",
                 "import pyqtorch.modules as pyq"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Fitting a 1D function\n",
-                "\n",
                 "Let's define a target function we want to fit."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {},
```

### Comparing `pyqtorch-0.2.6/docs/getting_started.ipynb` & `pyqtorch-0.2.7/docs/deprecated/getting_started.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.6/docs/deprecated/QAOA.ipynb` & `pyqtorch-0.2.7/docs/deprecated/QAOA.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.6/docs/deprecated/bench.py` & `pyqtorch-0.2.7/docs/deprecated/bench.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.6/docs/deprecated/fit_function.ipynb` & `pyqtorch-0.2.7/docs/deprecated/fit_function.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.6/docs/deprecated/ham_evol_comparison.ipynb` & `pyqtorch-0.2.7/docs/deprecated/ham_evol_comparison.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.6/docs/deprecated/state_evolution.ipynb` & `pyqtorch-0.2.7/docs/deprecated/state_evolution.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.6/pyqtorch/__init__.py` & `pyqtorch-0.2.7/pyqtorch/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.6/pyqtorch/ansatz.py` & `pyqtorch-0.2.7/pyqtorch/ansatz.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.6/pyqtorch/embedding.py` & `pyqtorch-0.2.7/pyqtorch/embedding.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.6/pyqtorch/matrices.py` & `pyqtorch-0.2.7/pyqtorch/matrices.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.6/pyqtorch/matrices_sparse.py` & `pyqtorch-0.2.7/pyqtorch/matrices_sparse.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.6/pyqtorch/converters/store_ops.py` & `pyqtorch-0.2.7/pyqtorch/converters/store_ops.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.6/pyqtorch/converters/to_qiskit.py` & `pyqtorch-0.2.7/pyqtorch/converters/to_qiskit.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.6/pyqtorch/core/__init__.py` & `pyqtorch-0.2.7/pyqtorch/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.6/pyqtorch/core/batched_operation.py` & `pyqtorch-0.2.7/pyqtorch/core/batched_operation.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.6/pyqtorch/core/circuit.py` & `pyqtorch-0.2.7/pyqtorch/core/circuit.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.6/pyqtorch/core/measurement.py` & `pyqtorch-0.2.7/pyqtorch/core/measurement.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.6/pyqtorch/core/operation.py` & `pyqtorch-0.2.7/pyqtorch/core/operation.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.6/pyqtorch/core/utils.py` & `pyqtorch-0.2.7/pyqtorch/core/utils.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.6/pyqtorch/modules/circuit.py` & `pyqtorch-0.2.7/pyqtorch/modules/circuit.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.6/pyqtorch/modules/hamevo.py` & `pyqtorch-0.2.7/pyqtorch/modules/hamevo.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.6/pyqtorch/modules/parametric.py` & `pyqtorch-0.2.7/pyqtorch/modules/parametric.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.6/pyqtorch/modules/primitive.py` & `pyqtorch-0.2.7/pyqtorch/modules/primitive.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.6/tests/conftest.py` & `pyqtorch-0.2.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.6/tests/test_batched_operations.py` & `pyqtorch-0.2.7/tests/test_batched_operations.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.6/tests/test_converters.py` & `pyqtorch-0.2.7/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.6/tests/test_module_hamevo.py` & `pyqtorch-0.2.7/tests/test_module_hamevo.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.6/tests/test_modules.py` & `pyqtorch-0.2.7/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.6/tests/test_operations.py` & `pyqtorch-0.2.7/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.6/tests/test_operations_hamevo.py` & `pyqtorch-0.2.7/tests/test_operations_hamevo.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.6/LICENSE` & `pyqtorch-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.6/pyproject.toml` & `pyqtorch-0.2.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     { name = "Aleksander Wennersteen", email = "aleksander.wennersteen@pasqal.com" },
     { name = "Mario Dagrada", email = "mario.dagrada@pasqal.com" },
     { name = "Dominik Seitz", email = "dominik.seitz@pasqal.com" },
     { name = "Niklas Heim", email = "niklas.heim@pasqal.com" },
 ]
 requires-python = ">=3.8.1,<3.11"
 license = {text = "Proprietary"}
-version = "0.2.6"
+version = "0.2.7"
 classifiers=[
     "License :: Other/Proprietary License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
@@ -27,25 +27,26 @@
 ]
 dependencies = [
     "openfermion>=1.5",
     "torch"
 ]
 
 [project.optional-dependencies]
-dev = ["black", "pytest", "pytest-cov", "flake8", "mypy", "pre-commit", "ruff"]
+dev = ["black", "pytest", "pytest-xdist", "pytest-cov", "flake8", "mypy", "pre-commit", "ruff", "nbconvert",
+  "ipykernel"]
 converters = ["qiskit"]
 
 [tool.hatch.envs.tests]
 features = [
   "dev",
   "converters",
 ]
 
 [tool.hatch.envs.tests.scripts]
-test = "pytest {args} && hatch -e docs run mkdocs build --clean --strict"
+test = "pytest -n auto {args} && hatch -e docs run mkdocs build --clean --strict"
 
 [tool.hatch.envs.docs]
 dependencies = [
   "mkdocs",
   "mkdocs-material",
   "mkdocstrings",
   "mkdocstrings-python",
```

### Comparing `pyqtorch-0.2.6/PKG-INFO` & `pyqtorch-0.2.7/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqtorch
-Version: 0.2.6
+Version: 0.2.7
 Summary: An efficient, large-scale emulator designed for quantum machine learning, seamlessly integrated with a PyTorch backend. Please refer to https://pyqtorch.readthedocs.io/en/latest/ for setup and usage info, along with the full documentation.
 Author-email: Slimane Thabet <slimane.thabet@pasqal.com>, Aleksander Wennersteen <aleksander.wennersteen@pasqal.com>, Mario Dagrada <mario.dagrada@pasqal.com>, Dominik Seitz <dominik.seitz@pasqal.com>, Niklas Heim <niklas.heim@pasqal.com>
 License: Proprietary
 License-File: LICENSE
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -17,12 +17,15 @@
 Requires-Dist: openfermion>=1.5
 Requires-Dist: torch
 Provides-Extra: converters
 Requires-Dist: qiskit; extra == 'converters'
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: flake8; extra == 'dev'
+Requires-Dist: ipykernel; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
+Requires-Dist: nbconvert; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: pytest-cov; extra == 'dev'
+Requires-Dist: pytest-xdist; extra == 'dev'
 Requires-Dist: ruff; extra == 'dev'
```

