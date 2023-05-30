# Comparing `tmp/signax-0.1.1.tar.gz` & `tmp/signax-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signax-0.1.1.tar", last modified: Tue Sep 27 12:42:07 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `signax-0.1.1.tar` & `signax-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 12:42:07.259147 signax-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-09-27 12:41:57.000000 signax-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4686 2022-09-27 12:42:07.259147 signax-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3751 2022-09-27 12:41:57.000000 signax-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-27 12:42:07.259147 signax-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1877 2022-09-27 12:41:57.000000 signax-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 12:42:07.255147 signax-0.1.1/signax/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-09-27 12:41:57.000000 signax-0.1.1/signax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      781 2022-09-27 12:41:57.000000 signax-0.1.1/signax/module.py
--rw-r--r--   0 runner    (1001) docker     (121)     4074 2022-09-27 12:41:57.000000 signax-0.1.1/signax/signature.py
--rw-r--r--   0 runner    (1001) docker     (121)     1736 2022-09-27 12:41:57.000000 signax-0.1.1/signax/signature_flattened.py
--rw-r--r--   0 runner    (1001) docker     (121)     4644 2022-09-27 12:41:57.000000 signax-0.1.1/signax/tensor_ops.py
--rw-r--r--   0 runner    (1001) docker     (121)     3390 2022-09-27 12:41:57.000000 signax-0.1.1/signax/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 12:42:07.255147 signax-0.1.1/signax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4686 2022-09-27 12:42:07.000000 signax-0.1.1/signax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      393 2022-09-27 12:42:07.000000 signax-0.1.1/signax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-27 12:42:07.000000 signax-0.1.1/signax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-27 12:42:07.000000 signax-0.1.1/signax.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-09-27 12:42:07.000000 signax-0.1.1/signax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-09-27 12:42:07.000000 signax-0.1.1/signax.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 12:42:07.259147 signax-0.1.1/test/
--rw-r--r--   0 runner    (1001) docker     (121)     2335 2022-09-27 12:41:57.000000 signax-0.1.1/test/test_signature.py
--rw-r--r--   0 runner    (1001) docker     (121)     4196 2022-09-27 12:41:57.000000 signax-0.1.1/test/test_tensor_ops.py
--rw-r--r--   0 runner    (1001) docker     (121)      570 2022-09-27 12:41:57.000000 signax-0.1.1/test/test_utils.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 signax-0.1.2/.git_archival.txt
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 signax-0.1.2/.gitattributes
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 signax-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 signax-0.1.2/.readthedocs.yml
+-rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 signax-0.1.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 signax-0.1.2/noxfile.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 signax-0.1.2/.github/dependabot.yml
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 signax-0.1.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0    30518 2020-02-02 00:00:00.000000 signax-0.1.2/assets/backward_cpu.png
+-rw-r--r--   0        0        0    29589 2020-02-02 00:00:00.000000 signax-0.1.2/assets/backward_gpu.png
+-rw-r--r--   0        0        0    29425 2020-02-02 00:00:00.000000 signax-0.1.2/assets/forward_cpu.png
+-rw-r--r--   0        0        0    30986 2020-02-02 00:00:00.000000 signax-0.1.2/assets/forward_gpu.png
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 signax-0.1.2/docs/conf.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 signax-0.1.2/docs/index.rst
+-rw-r--r--   0        0        0    48196 2020-02-02 00:00:00.000000 signax-0.1.2/examples/compare.ipynb
+-rw-r--r--   0        0        0    23963 2020-02-02 00:00:00.000000 signax-0.1.2/examples/estimate_hurst.ipynb
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 signax-0.1.2/examples/fbm.py
+-rw-r--r--   0        0        0   525790 2020-02-02 00:00:00.000000 signax-0.1.2/examples/generative_model.ipynb
+-rw-r--r--   0        0        0    43878 2020-02-02 00:00:00.000000 signax-0.1.2/examples/inversion.ipynb
+-rw-r--r--   0        0        0    12578 2020-02-02 00:00:00.000000 signax-0.1.2/examples/nets.py
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 signax-0.1.2/examples/utils/brownian_motion.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 signax-0.1.2/examples/utils/dataloader.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 signax-0.1.2/examples/utils/ornstein_uhlenbeck.py
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 signax-0.1.2/examples/utils/signature_normalization.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 signax-0.1.2/src/signax/__init__.py
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 signax-0.1.2/src/signax/module.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 signax-0.1.2/src/signax/py.typed
+-rw-r--r--   0        0        0     4024 2020-02-02 00:00:00.000000 signax-0.1.2/src/signax/signature.py
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 signax-0.1.2/src/signax/signature_flattened.py
+-rw-r--r--   0        0        0     4630 2020-02-02 00:00:00.000000 signax-0.1.2/src/signax/tensor_ops.py
+-rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 signax-0.1.2/src/signax/utils.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 signax-0.1.2/src/signax/_compat/__init__.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 signax-0.1.2/src/signax/_compat/typing.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 signax-0.1.2/tests/test_package.py
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 signax-0.1.2/tests/test_signature.py
+-rw-r--r--   0        0        0     4310 2020-02-02 00:00:00.000000 signax-0.1.2/tests/test_tensor_ops.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 signax-0.1.2/tests/test_utils.py
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 signax-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 signax-0.1.2/LICENSE
+-rw-r--r--   0        0        0     4226 2020-02-02 00:00:00.000000 signax-0.1.2/README.md
+-rw-r--r--   0        0        0     3929 2020-02-02 00:00:00.000000 signax-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 signax-0.1.2/PKG-INFO
```

### Comparing `signax-0.1.1/LICENSE` & `signax-0.1.2/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `signax-0.1.1/PKG-INFO` & `signax-0.1.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,32 @@
-Metadata-Version: 2.1
-Name: signax
-Version: 0.1.1
-Summary: Signax: Signature computation in JAX
-Home-page: https://github.com/anh-tong/signax
-Author: signax authors
-Author-email: anh.h.tong@gmail.com
-Maintainer: signax authors
-License: MIT
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Financial and Insurance Industry
-Classifier: Intended Audience :: Information Technology
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Requires-Python: ~=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Signax: Computing signatures in JAX
 
-[![CI](https://github.com/anh-tong/signax/actions/workflows/run-tests.yml/badge.svg)](https://github.com/anh-tong/signax/actions/workflows/run-tests.yml)
-![PyPI version](https://img.shields.io/pypi/v/signax)
+[![Actions Status][actions-badge]][actions-link]
+[![Documentation Status][rtd-badge]][rtd-link]
+[![PyPI version][pypi-version]][pypi-link]
+[![PyPI platforms][pypi-platforms]][pypi-link]
+
+<!-- prettier-ignore-start -->
+[actions-badge]:            https://github.com/Anh-Tong/signax/workflows/CI/badge.svg
+[actions-link]:             https://github.com/Anh-Tong/signax/actions
+[pypi-link]:                https://pypi.org/project/signax/
+[pypi-platforms]:           https://img.shields.io/pypi/pyversions/signax
+[pypi-version]:             https://img.shields.io/pypi/v/signax
+[rtd-badge]:                https://readthedocs.org/projects/signax/badge/?version=latest
+[rtd-link]:                 https://signax.readthedocs.io/en/latest/?badge=latest
+<!-- prettier-ignore-end -->
 
 ## Goal
 
-To have a library that supports signature computation in JAX. See [this paper](https://arxiv.org/abs/1905.08494) to see how to adopt signatures in machine learning.
-
-This implementation is inspired by [patrick-kidger/signatory](https://github.com/patrick-kidger/signatory).
+To have a library that supports signature computation in JAX. See
+[this paper](https://arxiv.org/abs/1905.08494) to see how to adopt signatures in
+machine learning.
 
+This implementation is inspired by
+[patrick-kidger/signatory](https://github.com/patrick-kidger/signatory).
 
 ## Examples
 
 Basic usage
 
 ```python
 import jax
@@ -69,54 +59,58 @@
 
 from signax.module import SignatureTransform
 
 # random generator key
 key = jrandom.PRNGKey(0)
 mlp_key, data_key = jrandom.split(key)
 
-depth=3
+depth = 3
 length, dim = 100, 3
 
 # we signature transfrom
 signature_layer = SignatureTransform(depth=depth)
-# finally, getting output via a neural network 
-last_layer = eqx.nn.MLP(depth=1, 
-                        in_size=3 + 3**2 + 3**3,
-                        width_size=4, 
-                        out_size=1,
-                        key=mlp_key)
+# finally, getting output via a neural network
+last_layer = eqx.nn.MLP(
+    depth=1, in_size=3 + 3**2 + 3**3, width_size=4, out_size=1, key=mlp_key
+)
 
 model = eqx.nn.Sequential(layers=[signature_layer, last_layer])
 x = jrandom.normal(shape=(length, dim), key=data_key)
 output = model(x)
 ```
 
-Also, check notebooks in `examples` folder for some experiments of [deep signature transforms paper](https://arxiv.org/abs/1905.08494).
+Also, check notebooks in `examples` folder for some experiments of
+[deep signature transforms paper](https://arxiv.org/abs/1905.08494).
+
 ## Installation
 
 Via pip
+
 ```
 pip install signax
 ```
 
 Via source
+
 ```
 git clone https://github.com/anh-tong/signax.git
 cd signax
 python setup.py install .
 ```
 
+## Parallelism
 
-## Parallelism 
+This implementation makes use of `jax.vmap` to perform the parallelism over
+batch dimension.
 
-This implementation makes use of `jax.vmap` to perform the parallelism over batch dimension. 
+Paralelism over chunks of paths is done using `jax.vmap` as well.
 
-Paralelism over chunks of paths is done using `jax.vmap` as well. 
-
-A quick comparison can be found at in the notebook `examples/compare.ipynb`. Below plots are comparison of forward and backward pass in both GPU and CPU for path `size=(32, 128, 8)` and signature `depth=5`
+A quick comparison can be found at in the notebook `examples/compare.ipynb`.
+Below plots are comparison of forward and backward pass in both GPU and CPU for
+path `size=(32, 128, 8)` and signature `depth=5`
 
 <table>
 <thead>
   <tr>
     <th >Forward</th>
     <th > Backward</th>
   </tr>
@@ -139,17 +133,23 @@
     </td>
   </tr>
 </tbody>
 </table>
 
 ## Why is using pure JAX good enough?
 
-Because JAX make use of just-in-time (JIT) compilations with XLA, Signax can be reasonably fast. 
+Because JAX make use of just-in-time (JIT) compilations with XLA, Signax can be
+reasonably fast.
 
-We observe that the performance of this implementation is similar to Signatory in CPU and slightly better in GPU. It could be because of the optimized operators of XLA in JAX. Note that [Signatory](https://github.com/patrick-kidger/signatory) contains highly optimized C++ source code (PyTorch with Pybind11).
+We observe that the performance of this implementation is similar to Signatory
+in CPU and slightly better in GPU. It could be because of the optimized
+operators of XLA in JAX. Note that
+[Signatory](https://github.com/patrick-kidger/signatory) contains highly
+optimized C++ source code (PyTorch with Pybind11).
 
 ## Acknowledgement
 
 This repo is based on
+
 - [Signatory](https://github.com/patrick-kidger/signatory)
 - [Deep-Signature-Transforms](https://github.com/patrick-kidger/Deep-Signature-Transforms)
 - [Equinox](https://github.com/patrick-kidger/equinox)
```

### Comparing `signax-0.1.1/signax/module.py` & `signax-0.1.2/src/signax/module.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,31 @@
-from typing import Optional
+from __future__ import annotations
 
 import equinox as eqx
-import jax.numpy as jnp
+import jax
+
 from signax.signature_flattened import signature, signature_combine
 
 
 class SignatureTransform(eqx.Module):
     depth: int
 
     def __init__(self, depth: int):
         self.depth = depth
 
     def __call__(
         self,
-        path: jnp.ndarray,
-        *,
-        key: Optional["jax.random.PRNGKey"] = None,  # noqa: F821
-    ) -> jnp.ndarray:
+        path: jax.Array,
+    ) -> jax.Array:
         return signature(path, self.depth)
 
 
 class SignatureCombine(eqx.Module):
     dim: int
     depth: int
 
     def __init__(self, dim: int, depth: int):
         self.dim = dim
         self.depth = depth
 
-    def __call__(self, signature1: jnp.ndarray, signature2: jnp.ndarray):
+    def __call__(self, signature1: jax.Array, signature2: jax.Array):
         return signature_combine(signature1, signature2, self.dim, self.depth)
```

### Comparing `signax-0.1.1/signax/signature.py` & `signax-0.1.2/src/signax/signature.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
+from __future__ import annotations
+
 from functools import partial
-from typing import List
 
 import jax
 import jax.numpy as jnp
 
 from .tensor_ops import log, mult, mult_fused_restricted_exp, restricted_exp
 from .utils import compress, lyndon_words
 
 
 @partial(jax.jit, static_argnames="depth")
-def signature(path: jnp.ndarray, depth: int) -> List[jnp.ndarray]:
+def signature(path: jax.Array, depth: int) -> list[jax.Array]:
     """
     Compute the signature of a path
 
     Args:
         path: size (length, dim)
         depth: signature is truncated at this depth
     Returns:
@@ -21,29 +22,28 @@
         [(dim, ), (dim, dim), (dim, dim, dim), ...]
     """
 
     path_increments = jnp.diff(path, axis=0)
     exp_term = restricted_exp(path_increments[0], depth=depth)
 
     def _body(i, val):
-        ret = mult_fused_restricted_exp(path_increments[i], val)
-        return ret
+        return mult_fused_restricted_exp(path_increments[i], val)
 
     exp_term = jax.lax.fori_loop(
         lower=1,
         upper=path_increments.shape[0],
         body_fun=_body,
         init_val=exp_term,
     )
 
     return exp_term
 
 
 @partial(jax.jit, static_argnames=["depth", "n_chunks"])
-def signature_batch(path: jnp.ndarray, depth: int, n_chunks: int):
+def signature_batch(path: jax.Array, depth: int, n_chunks: int):
     """Compute signature for a long path
 
     The path will be divided into chunks. The numbers of chunks
     is set manually.
 
     Args:
         path: size (length, dim)
@@ -58,40 +58,40 @@
     bulk_length = length - remainder
 
     path_bulk = path[1:bulk_length]
     path_bulk = jnp.reshape(path_bulk, (n_chunks, chunk_length, dim))
     basepoints = jnp.roll(path_bulk[:, -1], shift=1, axis=0)
     basepoints = basepoints.at[0].set(path[0])
     path_bulk = jnp.concatenate([basepoints[:, None, :], path_bulk], axis=1)
-    path_remainder = path[bulk_length - 1 :]  # noqa
+    path_remainder = path[bulk_length - 1 :]
 
     def _signature(path):
         return signature(path, depth)
 
     # this will return a list of [(b, n), (b, n, n), ...]
     multi_signatures = jax.vmap(_signature)(path_bulk)
     bulk_signature = multi_signature_combine(multi_signatures)
 
     if remainder != 0:
         # compute the signature of the remainder chunk
         remainder_signature = signature(path_remainder, depth)
         # combine with the bulk signature
         return mult(bulk_signature, remainder_signature)
-    else:
-        # no remainder, just return the bulk
-        return bulk_signature
+
+    # no remainder, just return the bulk
+    return bulk_signature
 
 
 def logsignature(path, depth):
     return signature_to_logsignature(signature(path, depth))
 
 
 def signature_to_logsignature(
-    signature: List[jnp.ndarray],
-) -> List[jnp.ndarray]:
+    signature: list[jax.Array],
+) -> list[jax.Array]:
     """
     Compute logsignature from signature
 
     This function ONLY supports the compression of expanded logsignature
     in Lyndon basis
 
     Args:
@@ -106,27 +106,26 @@
 
     indices = lyndon_words(depth, dim)
 
     # compute Lyndon words given `depth` and `dim`
     expanded_logsignature = log(signature)
 
     # compress using the information of Lyndon words
-    log_sig = compress(expanded_logsignature, indices)
-    return log_sig
+    return compress(expanded_logsignature, indices)
 
 
 def signature_combine(
-    signature1: List[jnp.ndarray],
-    signature2: List[jnp.ndarray],
+    signature1: list[jax.Array],
+    signature2: list[jax.Array],
 ):
     return mult(signature1, signature2)
 
 
 @jax.jit
-def multi_signature_combine(signatures: List[jnp.ndarray]):
+def multi_signature_combine(signatures: list[jax.Array]) -> list[jax.Array]:
     """
     Combine multiple signatures.
 
     The input of this function is the output of `jax.vmap` version of
     signature function.
 
     Args:
```

### Comparing `signax-0.1.1/signax/signature_flattened.py` & `signax-0.1.2/src/signax/signature_flattened.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
+from __future__ import annotations
+
 from functools import partial
 
 import jax
-import jax.numpy as jnp
 
 from .signature import logsignature as _logsignature
 from .signature import signature as _signature
 from .signature import signature_combine as _signature_combine
 from .signature import signature_to_logsignature as _signature_to_logsignature
 from .utils import flatten, unravel_signature
 
 
 @partial(jax.jit, static_argnames="depth")
-def signature(path: jnp.ndarray, depth: int) -> jnp.ndarray:
+def signature(path: jax.Array, depth: int) -> jax.Array:
     """
     Compute the signature of a path
 
     Args:
         path: size (length, dim)
         depth: signature is truncated at this depth
     Returns:
@@ -26,17 +27,15 @@
     return flatten(_signature(path, depth))
 
 
 def logsignature(path, depth):
     return flatten(_logsignature(path, depth))
 
 
-def signature_to_logsignature(
-    signature: jnp.ndarray, dim: int, depth: int
-) -> jnp.ndarray:
+def signature_to_logsignature(signature: jax.Array, dim: int, depth: int) -> jax.Array:
     """
     Compute logsignature from signature
 
     This function ONLY supports the compression of expanded logsignature
     in Lyndon basis
 
     Args:
@@ -48,12 +47,12 @@
     """
 
     unraveled = unravel_signature(signature, dim, depth)
     return flatten(_signature_to_logsignature(unraveled))
 
 
 def signature_combine(
-    signature1: jnp.ndarray, signature2: jnp.ndarray, dim: int, depth: int
-) -> jnp.ndarray:
+    signature1: jax.Array, signature2: jax.Array, dim: int, depth: int
+) -> jax.Array:
     sig1 = unravel_signature(signature1, dim, depth)
     sig2 = unravel_signature(signature2, dim, depth)
     return flatten(_signature_combine(sig1, sig2))
```

### Comparing `signax-0.1.1/signax/tensor_ops.py` & `signax-0.1.2/src/signax/tensor_ops.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,41 @@
+from __future__ import annotations
+
 from functools import partial
-from typing import List
 
 import jax
 import jax.numpy as jnp
 
 
 @jax.jit
-def otimes(x: jnp.ndarray, y: jnp.ndarray) -> jnp.ndarray:
+def otimes(x: jax.Array, y: jax.Array) -> jax.Array:
     """Tensor product
 
     Args:
         x: size=(n,n,...,n), ndim=ndim_x
         y: size=(n,n,...,n), ndim=ndim_y
     Return:
         Tensor size (n,n,...,n) with ndim=ndim_x + ndim_y
     """
     expanded_x = jnp.reshape(x, x.shape + (1,) * y.ndim)
     expanded_y = jnp.reshape(y, (1,) * x.ndim + y.shape)
     return expanded_x * expanded_y
 
 
 @jax.jit
-def addcmul(x: jnp.ndarray, y: jnp.ndarray, z: jnp.ndarray):
+def addcmul(x: jax.Array, y: jax.Array, z: jax.Array) -> jax.Array:
     """Similar to `torch.addcmul` returning
         x + y * z
     Here `*` is the tensor product
     """
     return x + otimes(y, z)
 
 
 @partial(jax.jit, static_argnames="depth")
-def restricted_exp(input: jnp.ndarray, depth: int) -> List[jnp.ndarray]:
+def restricted_exp(input: jax.Array, depth: int) -> list[jax.Array]:
     """Restricted exponentiate
 
     As `depth` is fixed so we can make it as a static argument.
     This allows us to `jit` this function
     Args:
         input: shape (n, )
         depth: the depth of signature
@@ -44,44 +45,42 @@
     ret = [input]
     for i in range(2, depth + 1):
         ret.append(otimes(ret[-1], input / i))
     return ret
 
 
 @jax.jit
-def mult_fused_restricted_exp(
-    z: jnp.ndarray, A: List[jnp.ndarray]
-) -> List[jnp.ndarray]:
+def mult_fused_restricted_exp(z: jax.Array, A: list[jax.Array]) -> list[jax.Array]:
     """
     Multiply-fused-exponentiate
 
     Args:
         z: shape (n,)
         A: a list of `jnp.array` [(n, ), (n x n), (n x n x n), ...]
     Return:
         A list of which elements have the same shape with `A`
     """
     depth = len(A)
     ret = []
 
     for depth_index in range(depth):
-        current = 1.0
+        current = jnp.array(1.0)
         for i in range(depth_index + 1):
             current = addcmul(x=A[i], y=current, z=z / (depth_index + 1 - i))
         ret.append(current)
 
     return ret
 
 
 @partial(jax.jit, static_argnums=2)
 def mult_inner(
-    A: List[jnp.ndarray],
-    B: List[jnp.ndarray],
+    A: list[jax.Array],
+    B: list[jax.Array],
     depth_index: int,
-) -> List[jnp.ndarray]:
+) -> list[jax.Array]:
     """
     Let `depth_index` = n
 
     this function returns
         $sum_{i=1}^n A_i x B_{n - i}$
 
 
@@ -99,15 +98,15 @@
             )
             for i in range(depth_index)
         ]
     )
 
 
 @jax.jit
-def mult(A: List[jnp.ndarray], B: List[jnp.ndarray]) -> List[jnp.ndarray]:
+def mult(A: list[jax.Array], B: list[jax.Array]) -> list[jax.Array]:
     """
     Multiplication in tensor algebra
 
     Args:
         A: [(dim,), (dim,dim), (dim,dim,dim), ...]
         B: [(dim,), (dim,dim), (dim,dim,dim), ...]
     """
@@ -118,19 +117,19 @@
         C[i] += mult_inner(A, B, depth_index=i)
 
     return C
 
 
 @partial(jax.jit, static_argnums=3)
 def mult_partial(
-    input1: List[jnp.ndarray],
-    input2: List[jnp.ndarray],
+    input1: list[jax.Array],
+    input2: list[jax.Array],
     scalar_term_value: float,
     top_terms_to_skip: int,
-) -> List[jnp.ndarray]:
+) -> list[jax.Array]:
     """Sort of multiplication in the tensor algebra
 
     `input1` assumed scalar value
     `input2` assume scalar value zero
 
     return `input1` x `input2` for some of its terms
 
@@ -153,15 +152,15 @@
 def _log_coef_at_depth(depth: int) -> float:
     """Note that reciprocals is an array [1/2, 1/3, ...]"""
     sign = -1.0 if depth % 2 == 0 else 1.0
     return sign / (depth + 2)
 
 
 @jax.jit
-def log(input: List[jnp.ndarray]) -> List[jnp.ndarray]:
+def log(input: list[jax.Array]) -> list[jax.Array]:
     """This follows Equation (10) of iisignature paper"""
 
     depth = len(input)
     if depth == 1:
         return input
 
     output = [jnp.zeros_like(x) for x in input]
```

### Comparing `signax-0.1.1/signax/utils.py` & `signax-0.1.2/src/signax/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+from __future__ import annotations
+
 from collections import defaultdict
 from functools import partial
-from typing import List, Tuple
+from typing import cast
 
 import jax
 import jax.numpy as jnp
 
 
 @jax.jit
-def index_select(input: jnp.ndarray, indices: jnp.ndarray) -> jnp.ndarray:
+def index_select(input: jax.Array, indices: jax.Array) -> jax.Array:
     """
     Select entries in m-level tensor based on given indices
     This function will help compressing log-signatures
 
     Args:
         input: size (dim, dim, ..., dim)
         indices: size (dim, n)
@@ -24,28 +26,28 @@
     n = indices.shape[1]
     assert n <= ndim
     strides = jnp.array([dim**i for i in range(n)])
     # flatten matrix A in C-style
     flattened = input.ravel()
     strides = jnp.array([dim**i for i in range(n)])
     # flatten matrix A in Fortran-style
-    flattened = input.flatten("F")
+    flattened = input.ravel("F")
 
-    def _select(index):
+    def _select(index: jax.Array) -> jax.Array:
         """index is a `jnp.ndarray` int"""
 
         # this is the way to compute the position of
         # (C-style) raveled arrays
         position = jnp.sum(index * strides)
         return flattened[position]
 
     return jax.vmap(_select)(indices)
 
 
-def lyndon_words(depth: int, dim: int) -> List[jnp.ndarray]:
+def lyndon_words(depth: int, dim: int) -> list[jax.Array]:
     """Generate Lyndon words of length `depth` over an `dim`-symbol alphabet
     Example in Python: https://gist.github.com/dvberkel/1950267
 
     Args:
         depth: int
         dim: int
     """
@@ -61,17 +63,17 @@
         while word and word[-1] == dim - 1:
             word.pop()
 
     return [jnp.stack(list_of_words[i]) for i in range(depth)]
 
 
 def compress(
-    input: List[jnp.ndarray],
-    indices: List[jnp.ndarray],
-) -> List[jnp.ndarray]:
+    input: list[jax.Array],
+    indices: list[jax.Array],
+) -> list[jax.Array]:
     """
     Compress expanded log-signatures using Lydon words
 
     Args:
         input: List of `jnp.ndarray`
         indices: generated by Lyndon words
 
@@ -79,56 +81,56 @@
         A list of compressed `jnp.ndarray`
     """
 
     return [index_select(term, index) for term, index in zip(input, indices)]
 
 
 @jax.jit
-def flatten(signature: List[jnp.ndarray]) -> jnp.ndarray:
+def flatten(signature: list[jax.Array]) -> jax.Array:
     flattened_terms = tuple(map(jnp.ravel, signature))
     return jnp.concatenate(flattened_terms)
 
 
 @partial(jax.jit, static_argnums=[0, 1])
-def _get_depth(dim: int, depth: int) -> Tuple:
+def _get_depth(dim: int, depth: int) -> tuple[jax.Array, jax.Array]:
     offset = jax.lax.integer_pow(dim, depth)
     start = dim * (1 - offset) // (1 - dim)
 
     return offset, start
 
 
 @partial(jax.jit, static_argnums=[1, 2, 3, 4])
 def _term_at(
-    flattened_signature: jnp.ndarray,
+    flattened_signature: jax.Array,
     dim: int,
     term_i: int,
     start: int,
     offset: int,
-) -> jnp.ndarray:
+) -> jax.Array:
     return jax.lax.dynamic_slice(
         flattened_signature,
         (start,),
         (offset,),
     ).reshape((term_i + 1) * (dim,))
 
 
 def term_at(
-    flattened_signature: jnp.ndarray,
+    flattened_signature: jax.Array,
     dim: int,
     term_i: int,
-) -> jnp.ndarray:
+) -> jax.Array:
     start, prev_offset = _get_depth(dim, term_i)
 
-    return _term_at(flattened_signature, dim, term_i, start, prev_offset * dim)
+    return cast(
+        jax.Array, _term_at(flattened_signature, dim, term_i, start, prev_offset * dim)
+    )
 
 
-def unravel_signature(
-    signature: jnp.ndarray, dim: int, depth: int
-) -> List[jnp.ndarray]:
-    unraveled: List[jnp.ndarray] = []
+def unravel_signature(signature: jax.Array, dim: int, depth: int) -> list[jax.Array]:
+    unraveled: list[jax.Array] = []
     start, offset = 0, dim
 
     for term_i in range(depth):
         unraveled.append(_term_at(signature, dim, term_i, start, offset))
         start += offset
         offset *= dim
```

### Comparing `signax-0.1.1/signax.egg-info/PKG-INFO` & `signax-0.1.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,75 @@
 Metadata-Version: 2.1
 Name: signax
-Version: 0.1.1
-Summary: Signax: Signature computation in JAX
-Home-page: https://github.com/anh-tong/signax
-Author: signax authors
-Author-email: anh.h.tong@gmail.com
-Maintainer: signax authors
-License: MIT
-Classifier: Development Status :: 3 - Alpha
+Version: 0.1.2
+Summary: Differentiable signature calculations in JAX.
+Project-URL: Homepage, https://github.com/Anh-Tong/signax
+Project-URL: Bug Tracker, https://github.com/Anh-Tong/signax/issues
+Project-URL: Discussions, https://github.com/Anh-Tong/signax/discussions
+Project-URL: Changelog, https://github.com/Anh-Tong/signax/releases
+Author-email: Anh Tong <anh.h.tong@gmail.com>
+License-File: LICENSE
+Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Financial and Insurance Industry
-Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Natural Language :: English
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Requires-Python: ~=3.7
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering
+Classifier: Typing :: Typed
+Requires-Python: >=3.8
+Requires-Dist: equinox
+Requires-Dist: jax>=0.3.10
+Requires-Dist: jaxlib
+Requires-Dist: typing-extensions>=3.7; python_version < '3.8'
+Provides-Extra: dev
+Requires-Dist: pytest-cov>=3; extra == 'dev'
+Requires-Dist: pytest>=6; extra == 'dev'
+Provides-Extra: docs
+Requires-Dist: furo; extra == 'docs'
+Requires-Dist: myst-parser>=0.13; extra == 'docs'
+Requires-Dist: sphinx-book-theme>=0.1.0; extra == 'docs'
+Requires-Dist: sphinx-copybutton; extra == 'docs'
+Requires-Dist: sphinx>=4.0; extra == 'docs'
+Provides-Extra: test
+Requires-Dist: pytest-cov>=3; extra == 'test'
+Requires-Dist: pytest>=6; extra == 'test'
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # Signax: Computing signatures in JAX
 
-[![CI](https://github.com/anh-tong/signax/actions/workflows/run-tests.yml/badge.svg)](https://github.com/anh-tong/signax/actions/workflows/run-tests.yml)
-![PyPI version](https://img.shields.io/pypi/v/signax)
+[![Actions Status][actions-badge]][actions-link]
+[![Documentation Status][rtd-badge]][rtd-link]
+[![PyPI version][pypi-version]][pypi-link]
+[![PyPI platforms][pypi-platforms]][pypi-link]
+
+<!-- prettier-ignore-start -->
+[actions-badge]:            https://github.com/Anh-Tong/signax/workflows/CI/badge.svg
+[actions-link]:             https://github.com/Anh-Tong/signax/actions
+[pypi-link]:                https://pypi.org/project/signax/
+[pypi-platforms]:           https://img.shields.io/pypi/pyversions/signax
+[pypi-version]:             https://img.shields.io/pypi/v/signax
+[rtd-badge]:                https://readthedocs.org/projects/signax/badge/?version=latest
+[rtd-link]:                 https://signax.readthedocs.io/en/latest/?badge=latest
+<!-- prettier-ignore-end -->
 
 ## Goal
 
-To have a library that supports signature computation in JAX. See [this paper](https://arxiv.org/abs/1905.08494) to see how to adopt signatures in machine learning.
-
-This implementation is inspired by [patrick-kidger/signatory](https://github.com/patrick-kidger/signatory).
+To have a library that supports signature computation in JAX. See
+[this paper](https://arxiv.org/abs/1905.08494) to see how to adopt signatures in
+machine learning.
 
+This implementation is inspired by
+[patrick-kidger/signatory](https://github.com/patrick-kidger/signatory).
 
 ## Examples
 
 Basic usage
 
 ```python
 import jax
@@ -69,54 +102,58 @@
 
 from signax.module import SignatureTransform
 
 # random generator key
 key = jrandom.PRNGKey(0)
 mlp_key, data_key = jrandom.split(key)
 
-depth=3
+depth = 3
 length, dim = 100, 3
 
 # we signature transfrom
 signature_layer = SignatureTransform(depth=depth)
-# finally, getting output via a neural network 
-last_layer = eqx.nn.MLP(depth=1, 
-                        in_size=3 + 3**2 + 3**3,
-                        width_size=4, 
-                        out_size=1,
-                        key=mlp_key)
+# finally, getting output via a neural network
+last_layer = eqx.nn.MLP(
+    depth=1, in_size=3 + 3**2 + 3**3, width_size=4, out_size=1, key=mlp_key
+)
 
 model = eqx.nn.Sequential(layers=[signature_layer, last_layer])
 x = jrandom.normal(shape=(length, dim), key=data_key)
 output = model(x)
 ```
 
-Also, check notebooks in `examples` folder for some experiments of [deep signature transforms paper](https://arxiv.org/abs/1905.08494).
+Also, check notebooks in `examples` folder for some experiments of
+[deep signature transforms paper](https://arxiv.org/abs/1905.08494).
+
 ## Installation
 
 Via pip
+
 ```
 pip install signax
 ```
 
 Via source
+
 ```
 git clone https://github.com/anh-tong/signax.git
 cd signax
 python setup.py install .
 ```
 
+## Parallelism
 
-## Parallelism 
+This implementation makes use of `jax.vmap` to perform the parallelism over
+batch dimension.
 
-This implementation makes use of `jax.vmap` to perform the parallelism over batch dimension. 
+Paralelism over chunks of paths is done using `jax.vmap` as well.
 
-Paralelism over chunks of paths is done using `jax.vmap` as well. 
-
-A quick comparison can be found at in the notebook `examples/compare.ipynb`. Below plots are comparison of forward and backward pass in both GPU and CPU for path `size=(32, 128, 8)` and signature `depth=5`
+A quick comparison can be found at in the notebook `examples/compare.ipynb`.
+Below plots are comparison of forward and backward pass in both GPU and CPU for
+path `size=(32, 128, 8)` and signature `depth=5`
 
 <table>
 <thead>
   <tr>
     <th >Forward</th>
     <th > Backward</th>
   </tr>
@@ -139,17 +176,23 @@
     </td>
   </tr>
 </tbody>
 </table>
 
 ## Why is using pure JAX good enough?
 
-Because JAX make use of just-in-time (JIT) compilations with XLA, Signax can be reasonably fast. 
+Because JAX make use of just-in-time (JIT) compilations with XLA, Signax can be
+reasonably fast.
 
-We observe that the performance of this implementation is similar to Signatory in CPU and slightly better in GPU. It could be because of the optimized operators of XLA in JAX. Note that [Signatory](https://github.com/patrick-kidger/signatory) contains highly optimized C++ source code (PyTorch with Pybind11).
+We observe that the performance of this implementation is similar to Signatory
+in CPU and slightly better in GPU. It could be because of the optimized
+operators of XLA in JAX. Note that
+[Signatory](https://github.com/patrick-kidger/signatory) contains highly
+optimized C++ source code (PyTorch with Pybind11).
 
 ## Acknowledgement
 
 This repo is based on
+
 - [Signatory](https://github.com/patrick-kidger/signatory)
 - [Deep-Signature-Transforms](https://github.com/patrick-kidger/Deep-Signature-Transforms)
 - [Equinox](https://github.com/patrick-kidger/equinox)
```

### Comparing `signax-0.1.1/test/test_tensor_ops.py` & `signax-0.1.2/tests/test_tensor_ops.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,34 @@
+from __future__ import annotations
+
 import jax
 import jax.numpy as jnp
 import numpy as np
 import signatory
 
 # need to install torch and signatory for testing
 import torch
+from numpy.random import default_rng
+
 from signax.signature import signature, signature_to_logsignature
 from signax.tensor_ops import (
     addcmul,
     mult,
     mult_fused_restricted_exp,
     otimes,
     restricted_exp,
 )
 
+rng = default_rng()
+
 
 jax.config.update("jax_platform_name", "cpu")
 
 
 def test_otimes():
-
     # 1D x 1D
     x = jnp.array([1.0, 2.0])
     y = jnp.array([3.0, 4.0])
 
     true_output = jnp.array([[3.0, 4.0], [6.0, 8.0]])
     assert jnp.allclose(true_output, otimes(x, y), rtol=1e-3, atol=1e-5)
 
@@ -46,27 +51,25 @@
         ]
     )
 
     assert jnp.allclose(true_output, otimes(y, x), rtol=1e-3, atol=1e-5)
 
 
 def test_addcmul():
-
     x = jnp.array([[1.0, 2.0], [3.0, 4.0]])
     y = jnp.array([1.0, 2.0])
     z = jnp.array([3.0, 4.0])
     true_output = jnp.array([[4.0, 6.0], [9.0, 12.0]])
     assert jnp.allclose(true_output, addcmul(x, y, z), rtol=1e-3, atol=1e-5)
 
 
 def test_restricted_exp():
-
     depth = 4
     length, dim = 2, 3
-    path = np.random.randn(length, dim)
+    path = rng.standard_normal((length, dim))
 
     signatory_output = (
         signatory.signature(
             torch.tensor(path)[None, ...],
             depth=depth,
         )
         .sum()
@@ -75,18 +78,17 @@
     jax_output = restricted_exp(jnp.diff(path, axis=0), depth=depth)
     jax_output = sum([jnp.sum(x) for x in jax_output])
     # only check the sum of output in two cases are the same
     assert jnp.allclose(signatory_output, jax_output, rtol=1e-3, atol=1e-5)
 
 
 def test_mult_fused_restricted_exp():
-
     depth = 4
     length, dim = 3, 3
-    path = np.random.randn(length, dim)
+    path = rng.standard_normal((length, dim))
 
     # re-test restricted_exp() to make sure it run correctly
     test_restricted_exp()
 
     signatory_output = (
         signatory.signature(
             torch.tensor(path)[None, ...],
@@ -102,18 +104,17 @@
     jax_output = mult_fused_restricted_exp(increments[1], exp_term)
     jax_output = sum([jnp.sum(x) for x in jax_output])
     # again, just check the sum
     assert jnp.allclose(signatory_output, jax_output, rtol=1e-3, atol=1e-5)
 
 
 def test_mult():
-
     depth = 4
     length, dim = 3, 4
-    path = np.random.randn(length, dim)
+    path = rng.standard_normal((length, dim))
 
     # use our implementation, need to compute exp first
     increments = jnp.diff(path, axis=0)
     exp1 = restricted_exp(increments[0], depth)
     exp2 = restricted_exp(increments[1], depth)
     combine = mult(exp1, exp2)
     jax_output = sum(jnp.sum(x) for x in combine)
@@ -132,15 +133,15 @@
     assert jnp.allclose(signatory_output, jax_output, rtol=1e-3, atol=1e-5)
 
 
 def test_log():
     """Test log via signature_to_logsignature"""
     depth = 4
     length, dim = 3, 2
-    path = np.random.randn(length, dim)
+    path = rng.standard_normal((length, dim))
     jax_path = jnp.array(path)
     jax_signature = signature(jax_path, depth)
     jax_logsignature = signature_to_logsignature(jax_signature)
 
     jax_output = sum(jnp.sum(x) for x in jax_logsignature)
     jax_output = jax_output.item()
```

### Comparing `signax-0.1.1/test/test_utils.py` & `signax-0.1.2/tests/test_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+from __future__ import annotations
+
 import jax.numpy as jnp
+
 from signax.utils import index_select
 
 
 def test_index_select():
-
     # first test
     dim = 4
     a = jnp.arange(0, dim**2).reshape((dim, dim))
     indices = jnp.array([[0, 0], [0, 1], [3, 3]])
     true_output = jnp.array([0, 1, 15])
     assert jnp.allclose(true_output, index_select(a, indices))
```

