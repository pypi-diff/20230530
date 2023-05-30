# Comparing `tmp/lmo-0.4.0.tar.gz` & `tmp/lmo-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmo-0.4.0.tar", max compression
+gzip compressed data, was "lmo-0.5.0.tar", max compression
```

## Comparing `lmo-0.4.0.tar` & `lmo-0.5.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1505 2023-04-29 15:29:38.675734 lmo-0.4.0/LICENSE
--rw-r--r--   0        0        0      772 2023-05-14 21:15:11.042568 lmo-0.4.0/README.md
--rw-r--r--   0        0        0      984 2023-05-19 18:57:02.754904 lmo-0.4.0/lmo/__init__.py
--rw-r--r--   0        0        0      158 2023-05-02 20:44:05.723493 lmo-0.4.0/lmo/_meta.py
--rw-r--r--   0        0        0      415 2023-05-14 01:14:00.711613 lmo-0.4.0/lmo/_utils.py
--rw-r--r--   0        0        0     9922 2023-05-20 21:05:10.190270 lmo-0.4.0/lmo/multivariate.py
--rw-r--r--   0        0        0        0 2023-04-29 15:53:33.056174 lmo-0.4.0/lmo/py.typed
--rw-r--r--   0        0        0     1099 2023-05-14 01:14:00.735614 lmo-0.4.0/lmo/stats.py
--rw-r--r--   0        0        0     1256 2023-05-19 18:51:37.495742 lmo-0.4.0/lmo/typing.py
--rw-r--r--   0        0        0    10176 2023-05-20 20:14:06.706453 lmo-0.4.0/lmo/univariate.py
--rw-r--r--   0        0        0     5583 2023-05-20 21:21:50.896584 lmo-0.4.0/lmo/weights.py
--rw-r--r--   0        0        0     1907 2023-05-20 21:20:31.986822 lmo-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1870 1970-01-01 00:00:00.000000 lmo-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1505 2023-04-29 15:29:38.675734 lmo-0.5.0/LICENSE
+-rw-r--r--   0        0        0      792 2023-05-30 00:24:12.512261 lmo-0.5.0/README.md
+-rw-r--r--   0        0        0      648 2023-05-29 17:01:54.387498 lmo-0.5.0/lmo/__init__.py
+-rw-r--r--   0        0        0      158 2023-05-02 20:44:05.723493 lmo-0.5.0/lmo/_meta.py
+-rw-r--r--   0        0        0     1618 2023-05-29 00:06:01.539181 lmo-0.5.0/lmo/_utils.py
+-rw-r--r--   0        0        0     3754 2023-05-29 19:26:06.023457 lmo-0.5.0/lmo/linalg.py
+-rw-r--r--   0        0        0    11828 2023-05-30 00:07:26.249912 lmo-0.5.0/lmo/multivariate.py
+-rw-r--r--   0        0        0        0 2023-04-29 15:53:33.056174 lmo-0.5.0/lmo/py.typed
+-rw-r--r--   0        0        0     4393 2023-05-29 19:14:01.515594 lmo-0.5.0/lmo/stats.py
+-rw-r--r--   0        0        0     1609 2023-05-29 19:12:59.718239 lmo-0.5.0/lmo/typing.py
+-rw-r--r--   0        0        0    12307 2023-05-29 22:01:31.773252 lmo-0.5.0/lmo/univariate.py
+-rw-r--r--   0        0        0     6670 2023-05-29 18:53:48.844937 lmo-0.5.0/lmo/weights.py
+-rw-r--r--   0        0        0     1981 2023-05-30 00:24:53.249167 lmo-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1890 1970-01-01 00:00:00.000000 lmo-0.5.0/PKG-INFO
```

### Comparing `lmo-0.4.0/LICENSE` & `lmo-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lmo-0.4.0/README.md` & `lmo-0.5.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -6,19 +6,13 @@
 
 ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/jorenham/lmo/CI.yml?branch=master&style=flat-square)
 [![PyPI](https://img.shields.io/pypi/v/lmo?style=flat-square)](https://pypi.org/project/lmo/)
 [![versions](https://img.shields.io/pypi/pyversions/lmo?style=flat-square)](https://github.com/jorenham/lmo)
 [![license](https://img.shields.io/github/license/jorenham/lmo?style=flat-square)](https://github.com/jorenham/lmo/blob/master/LICENSE?)
 
 
-Streamlined calculation of L-moments and TL-moments.
+Generalized trimmed **L-mo**ments for robust statistics. 
 
 ---
 <!--head-end-->
 
-[Documentation](https://jorenham.github.io/lmo/)
-
----
-
-*Examples coming soon*.
-
-
+See the [documentation](https://jorenham.github.io/lmo/) for usage examples and code reference.
```

### Comparing `lmo-0.4.0/lmo/typing.py` & `lmo-0.5.0/lmo/typing.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,66 @@
 __all__ = (
+    'AnyNDArray',
+
     'AnyBool',
     'AnyInt',
     'AnyFloat',
-    'AnyVector',
-    'AnyMatrix',
-    'AnyTensor',
-    'ScalarOrArray',
+
+    'IntVector',
+    'IntMatrix',
+    'IntTensor',
+
+    'FloatVector',
+    'FloatMatrix',
+    'FloatTensor',
+
     'SortKind',
-    'Trimming',
+    'IndexOrder',
 )
 
 from typing import (
     Any,
     Literal,
+    Protocol,
     Sequence,
-    SupportsFloat,
     TypeAlias,
     TypeVar,
+    runtime_checkable,
 )
 
 import numpy as np
+import numpy.typing as npt
 
-# scalar types
-AnyBool: TypeAlias = bool | np.bool_
-AnyInt: TypeAlias = int | np.integer[Any] | AnyBool
-AnyFloat: TypeAlias = float | np.floating[Any] | AnyInt
 
-_R = TypeVar('_R', bound=np.floating[Any] | np.integer[Any] | np.bool_)
-_AnyR = TypeVar('_AnyR', bound=SupportsFloat)
+T = TypeVar('T', bound=np.generic)
+T_co = TypeVar('T_co', covariant=True, bound=np.generic)
+
+@runtime_checkable
+class _SupportsArray(Protocol[T_co]):
+    def __array__(self) -> npt.NDArray[T_co]: ...
+
+
+# scalar types
+_NumpyBool: TypeAlias = np.bool_
+_NumpyInteger: TypeAlias = np.integer[Any] | _NumpyBool
+_NumpyFloating: TypeAlias = np.floating[Any] | _NumpyInteger
+
+AnyBool: TypeAlias = _NumpyBool | bool
+AnyInt: TypeAlias = _NumpyInteger | int | bool
+AnyFloat: TypeAlias = _NumpyFloating | float | int | bool
 
 # array-like flavours (still waiting on numpy's shape typing)
-AnyVector: TypeAlias = np.ndarray[Any, np.dtype[Any]] | Sequence[SupportsFloat]
-AnyMatrix: TypeAlias = AnyVector | Sequence[AnyVector]
-AnyTensor: TypeAlias = AnyMatrix | Sequence['AnyTensor']
+AnyNDArray: TypeAlias = npt.NDArray[T] | _SupportsArray[T]
+
+IntVector: TypeAlias = AnyNDArray[_NumpyInteger] | Sequence[AnyInt]
+IntMatrix: TypeAlias = AnyNDArray[_NumpyInteger] | Sequence[IntVector]
+IntTensor: TypeAlias = AnyNDArray[_NumpyInteger] | Sequence['IntTensor']
+
+FloatVector: TypeAlias = AnyNDArray[_NumpyFloating] | Sequence[AnyFloat]
+FloatMatrix: TypeAlias = AnyNDArray[_NumpyFloating] | Sequence[FloatVector]
+FloatTensor: TypeAlias = AnyNDArray[_NumpyFloating] | Sequence['FloatTensor']
+
 
-# complex numbers aren't relevant (and calling them scalars is far-fetched IMHO)
-ScalarOrArray: TypeAlias = _R | np.ndarray[Any, np.dtype[_R]]
 
 # for numpy.sort
-SortKind: TypeAlias = Literal[
-    'quicksort',
-    'mergesort',
-    'heapsort',
-    'stable',
-] | None
-
-# trim length
-_Trim0: TypeAlias = tuple[()]
-_Trim1: TypeAlias = tuple[int] | int
-_Trim2: TypeAlias = tuple[int, int]
-Trimming: TypeAlias = _Trim0 | _Trim1 | _Trim2
+SortKind: TypeAlias = Literal['quicksort', 'heapsort', 'stable']
+IndexOrder: TypeAlias = Literal['C', 'F', 'A', 'K']
```

### Comparing `lmo-0.4.0/lmo/univariate.py` & `lmo-0.5.0/lmo/multivariate.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,377 +1,376 @@
-"""
-Estimators of the sample L- and TL-moments, and related summary statistics.
-"""
-
 __all__ = (
-    'l_moment',
-    'l_ratio',
-    'l_loc',
-    'l_scale',
-    'l_skew',
-    'l_kurt',
-
-    'tl_moment',
-    'tl_ratio',
-    'tl_loc',
-    'tl_scale',
-    'tl_skew',
-    'tl_kurt',
+    'l_comoment',
+    'l_coratio',
+    'l_coloc',
+    'l_coscale',
+    'l_corr',
+    'l_coskew',
+    'l_cokurtosis',
 )
 
-from typing import Any
+from typing import Any, TypeVar, cast
 
 import numpy as np
-import numpy.typing as npt
+from numpy import typing as npt
+
+from ._utils import clean_order
+from .stats import order_stats
+from .typing import AnyInt, IntVector, SortKind
+from .weights import l_weights
 
-from .typing import AnyTensor, ScalarOrArray, SortKind, Trimming
-from .weights import tl_weights, reweight
+T = TypeVar('T', bound=np.floating[Any])
 
 
-def tl_moment(
-    a: AnyTensor,
-    r: int,
+def l_comoment(
+    a: npt.ArrayLike,
+    r: AnyInt | IntVector,
     /,
-    trim: Trimming = 1,
-    axis: int | None = None,
+    trim: tuple[int, int] = (0, 0),
+    rowvar: bool = True,
+    dtype: np.dtype[T] | type[T] = np.float_,
     *,
-    weights: AnyTensor | None = None,
-    sort: SortKind = None,
-) -> ScalarOrArray[np.float_]:
+    sort: SortKind | None = 'stable',
+) -> npt.NDArray[T]:
     """
-    Estimate the $r$-th sample TL-moment, $\\lambda_{r}^{(t_1, t_2)}$, for
-    left and right trim lengths $t_1$ and $t_2$.
+    Multivariate extension of [`lmo.l_moment`][lmo.l_moment]. Estimates the
+    L-comoment matrix:
+
+    $$
+    \\Lambda_{r}^{(t_1, t_2)} =
+        \\left[
+            \\lambda_{r [ij]}^{(t_1, t_2)}
+        \\right]_{m \\times m}
+    $$
+
+    Whereas the L-moments are calculated using the order statistics of the
+    observations, i.e. by sorting, the L-comoment sorts $x_i$ using the
+    order of $x_j$. This means that in general,
+    $\\lambda_{r [ij]}^{(t_1, t_2)} \\neq \\lambda_{r [ji]}^{(t_1, t_2)}$, i.e.
+    $\\Lambda_{r}^{(t_1, t_2)}$ is not symmetric.
+
+    The $r$-th L-comoment $\\lambda_{r [ij]}^{(t_1, t_2)}$ reduces to the
+    L-moment if $i=j$, and can therefore be seen as a generalization of the
+    (univariate) L-moments. Similar to how the diagonal of a covariance matrix
+    contains the variances, the diagonal of the L-comoment matrix contains the
+    L-moments.
+
+    Based on the proposed definition by Serfling & Xiao (2007) for L-comoments.
+    Extended to allow for generalized trimming.
 
     Parameters:
-        a (array_like):
-            Array containing numbers whose TL-moment is desired. If `a` is not
-            an array, a conversion is attempted.
-
-        r (int):
-            The order of the TL-moment. Some special cases cases include
-
-            - `0`: Like the zeroth moment, the zeroth TL-moment  is always `1`.
-            - `1`: The TL-location, the analogue of the mean. See
-                [`tl_loc`][lmo.tl_loc].
-            - `2`: The TL-scale, analogous to the standard deviation. See
-                [`tl_scale`][lmo.tl_scale].
-
-        trim (int | tuple[int, int]):
-            Amount of samples to trim as either
-
-            - `t: int` for symmetric trimming, equivalent to `(t, t)`.
-            - `(t1: int, t2: int)` for asymmetric trimming, or
-
-            If `0` is passed, the L-moment is returned.
-
-        axis (int?):
-            Axis along wich to calculate the TL-moments.
-            If `None` (default), all samples in the array will be used.
-
-        weights (array_like, optional):
-            An array of weights associated with the values in `a`. Each value
-            in `a` contributes to the average according to its associated
-            weight.
-            The weights array can either be 1-D (in which case its length must
-            be the size of a along the given axis) or of the same shape as `a`.
-            If `weights=None`, then all data in `a` are assumed to have a
-            weight equal to one.
-
-            All `weights` must be `>=0`, and the sum must be nonzero.
-
-            The algorithm is similar to that of the weighted median. See
-            [`lmo.weights.reweight`][lmo.weights.reweight] for details.
-
-    Other parameters:
-        sort ('quick' | 'heap' | 'stable' | 'merge'):
-            Sorting algorithm, see [`numpy.sort`](
-            https://numpy.org/doc/stable/reference/generated/numpy.sort).
+        a:
+            1-D or 2-D array-like containing `m` variables and `n` observations.
+            Each row of `a` represents a variable, and each column a single
+            observation of all those variables. Also see `rowvar` below.
+            If `a` is not an array, a conversion is attempted.
+
+        r:
+            The L-moment order(s), non-negative integer or array.
+
+        trim:
+            Left- and right-trim orders $(t_1, t_2)$, non-negative integers
+            that are bound by $t_1 + t_2 < n - r$.
+
+            Some special cases include:
+
+            - $(0, 0)$: The original **L**-moment, introduced by Hosking (1990).
+                Useful for fitting the e.g. log-normal and generalized extreme
+                value (GEV) distributions.
+            - $(0, m)$: **LL**-moment (**L**inear combination of **L**owest
+                order statistics), instroduced by Bayazit & Onoz (2002).
+                Assigns more weight to smaller observations.
+            - $(s, 0)$: **LH**-moment (**L**inear combination of **H**igher
+                order statistics), by Wang (1997).
+                Assigns more weight to larger observations.
+            - $(t, t)$: **TL**-moment (**T**rimmed L-moment) $\\lambda_r^t$,
+                with symmetric trimming. First introduced by
+                Elamir & Seheult (2003).
+                Generally more robust than L-moments.
+                Useful for fitting heavy-tailed distributions, such as the
+                Cauchy distribution.
+
+        rowvar:
+            If `rowvar` is True (default), then each row (axis 0) represents a
+            variable, with observations in the columns (axis 1).
+            Otherwise, the relationship is transposed: each column represents
+            a variable, while the rows contain observations.
+
+        dtype:
+            Floating type to use in computing the L-moments. Default is
+            [`numpy.float64`][numpy.float64].
+
+        sort ('quick' | 'stable' | 'heap'):
+            Sorting algorithm, see [`numpy.sort`][numpy.sort].
 
     Returns:
-        Scalar or array; the $r$-th TL-moment(s).
+        L: Array of shape `(*r.shape, m, m)` with r-th L-comoments.
 
-    See Also:
-        - [E. Elmamir & A. Seheult (2003) - Trimmed L-moments](
-            https://doi.org/10.1016/S0167-9473(02)00250-5)
-        - [J.R.M. Hosking (2007) - Some theory and practical uses of trimmed
-            L-moments](https://doi.org/10.1016/j.jspi.2006.12.002)
-
-    """
-    x = np.asanyarray(a)
-    w_x = None if weights is None else np.asanyarray(weights)
-
-    # ensure that the samples are along the first axis (shape standardization)
-    # this way we don't have the bother with the specific axis from here on
-    if axis is None:
-        x = x.ravel()
-    if x.ndim > 1 and w_x is not None:
-        x, w_x = np.broadcast_arrays(x, w_x)
-    if axis and (ax := axis % x.ndim):
-        x = np.moveaxis(x, ax, 0)
-        if w_x is not None:
-            w_x = np.moveaxis(x, ax, 0)
-
-    n = len(x)
-
-    if r == 0:
-        # zeroth (TL-)moment is always 1
-        # the _[()] ensures that those annoying 0d "arrays" become scalars
-        return np.ones(x.shape[1:])[()]
-
-    # calculate the TL-weight vector (it anoly depends on n and r, not on the
-    # amount of variables)
-    w_r = tl_weights(n, r, trim)
-
-    def _apply_weights_1d(
-        _x: npt.NDArray[np.floating[Any]],
-        _w_x: npt.NDArray[Any] | None = None
-    ) -> npt.NDArray[np.float_]:
-        assert _x.ndim == 1
-        assert _w_x is None or _w_x.shape == _x.shape
-
-        if _w_x is None:
-            _x_k, _w = np.sort(_x, kind=sort), w_r
-        else:
-            i_k = np.argsort(_x, kind=sort)
-            _x_k, _w = _x[i_k], reweight(w_r, _w_x[i_k])
-
-        return _x_k @ _w
-
-    if x.ndim == 1:
-        return _apply_weights_1d(x, w_x)
-
-    if w_x is None:
-        return np.apply_along_axis(_apply_weights_1d, 0, x)
-
-    # manual version of numpy.apply_along_axis, which handles only one array
-    out = np.empty(x.shape[1:], dtype=np.result_type(x, w_r, w_x))
-    for jj in np.ndindex(*out.shape):
-        out[jj] = _apply_weights_1d(x[jj], w_x[jj])
-    return out
-
-
-def tl_ratio(
-    a: AnyTensor,
-    r: int,
-    /,
-    k: int = 2,
-    trim: Trimming = 1,
-    axis: int | None = None,
-    **kwargs: Any,
-) -> ScalarOrArray[np.float_]:
-    """
-    Ratio of the r-th and k-th (2nd by default) sample TL-moments:
+    Examples:
+        Estimation of the second L-comoment (the L-coscale) from biviariate
+        normal samples:
 
-    $$
-    \\tau_{r, k}^{(t_1, t_2)} = \\frac{
-        \\lambda_{r}^{(t_1, t_2)}
-    }{
-        \\lambda_{k}^{(t_1, t_2)}
-    }
-    $$
+        >>> import lmo, numpy as np
+        >>> rng = np.random.default_rng(12345)
+        >>> x = rng.multivariate_normal([0, 0], [[6, -3], [-3, 3.5]], 99).T
+        >>> lmo.l_comoment(x, 2)
+        array([[ 1.2766793 , -0.83299947],
+               [-0.71547941,  1.05990727]])
+
+        The diagonal contains the univariate L-moments:
+
+        >>> lmo.l_moment(x, 2, axis=-1)
+        array([1.2766793 , 1.05990727])
 
-    By default, $k = 2$ and $t_1 = t_2 = 1$ are used, i.e.
-    $\\tau_{r, 2}^{(1, 1)}$, or $\\tau_r^{(1)}$ for short.
+    References:
+        * [R. Serfling & P. Xiao (2007) - A Contribution to Multivariate
+            L-Moments: L-Comoment Matrices](https://doi.org/10.1016/j.jmva.2007.01.008)
 
     """
-    x = np.asanyarray(a)
+    def _clean_array(arr: npt.ArrayLike) -> npt.NDArray[T]:
+        out = np.asanyarray(arr, dtype=dtype)
+        return out if rowvar else out.T
 
-    l_r = tl_moment(x, r, trim, axis=axis, **kwargs)
+    x = np.atleast_2d(_clean_array(a))
+    if x.ndim != 2:
+        raise ValueError(f'sample array must be 2-D, got {x.ndim}')
 
-    if k == 0:
-        return l_r
-    if k == r:
-        return np.ones_like(l_r)[()]
+    _r = np.asarray(r)
+    r_max: int = clean_order(cast(
+        int,
+        np.max(_r)  # pyright: ignore [reportUnknownMemberType]
+    ))
+    m, n = x.shape
 
-    l_k = l_r if k == r else tl_moment(x, k, trim, axis=axis, **kwargs)
+    if not m:
+        return np.empty(np.shape(_r) + (0, 0), dtype=dtype)
 
-    # i.e. `x / 0 = 0 if x == 0 else np.nan`
-    return np.divide(
-        l_r,
-        l_k,
-        out=np.where(l_r == 0, 0.0, np.nan),
-        where=l_k != 0
-    )[()]  # [()] converts any 0-dimensional arrays to scalar
+    # projection matrix of shape (r, n)
+    P_r = l_weights(r_max, n, trim, dtype=dtype)
 
+    # L-comoment matrices for r = 0, ..., r_max
+    L_ij = np.empty((r_max + 1, m, m), dtype=dtype)
 
-def tl_loc(
-    a: AnyTensor,
-    /,
-    trim: Trimming = 1,
-    axis: int | None = None,
-    **kwargs: Any,
-) -> ScalarOrArray[np.float_]:
-    """
-    Sample estimator of the TL-location, $\\lambda_1^{(t_1, t_2)}$; the first
-    TL-moment.
+    # the zeroth L-comoment is the delta function, so the L-comoment
+    # matrix is the identity matrix
+    L_ij[0] = np.eye(m, dtype=dtype)
 
-    See Also:
-         [lmo.tl_moment][lmo.univariate.tl_moment]
-    """
-    return tl_moment(a, 1, trim, axis=axis, **kwargs)
+    kwargs = {'axis': -1, 'dtype': dtype, 'sort': sort}
+    for j in range(m):
+        # concomitants of x[i] w.r.t. x[j] for all i
+        x_k_ij = order_stats(x, x[j], **kwargs)
 
+        L_ij[1:, :, j] = np.inner(P_r, x_k_ij)
 
-def tl_scale(
-    a: AnyTensor,
-    /,
-    trim: Trimming = 1,
-    axis: int | None = None,
-    **kwargs: Any,
-) -> ScalarOrArray[np.float_]:
-    """
-    Sample TL-scale estimator, $\\lambda_2^{(t_1, t_2)}$, the second TL-moment.
-    A robust alternative of the sample standard deviation.
-    """
-    return tl_moment(a, 2, trim, axis=axis, **kwargs)
+    return L_ij.take(_r, 0)  # pyright: ignore [reportUnknownMemberType]
 
 
-def tl_skew(
-    a: AnyTensor,
+def l_coratio(
+    a: npt.ArrayLike,
+    r: AnyInt | IntVector,
+    s: AnyInt | IntVector,
     /,
-    trim: Trimming = 1,
-    axis: int | None = None,
+    trim: tuple[int, int] = (0, 0),
+    rowvar: bool = True,
+    dtype: np.dtype[T] | type[T] = np.float_,
     **kwargs: Any,
-) -> ScalarOrArray[np.float_]:
-    """
-    TL-skewness coefficient, $\\tau_3^{(t_1, t_2)}$; the 3rd sample TL-moment
-    ratio.
+) -> npt.NDArray[T]:
     """
-    return tl_ratio(a, 3, trim=trim, axis=axis, **kwargs)
+    Estimate the generalized matrix of L-comoment ratio's:
 
+    $$
+    \\tilde \\Lambda_{rs}^{(t_1, t_2)} =
+        \\left[
+            \\left. \\lambda_{r [ij]}^{(t_1, t_2)} \\right/
+            \\lambda_{s [jj]}^{(t_1, t_2)}
+        \\right]_{m \\times m}
+    $$
+
+    See Also:
+        - [`lmo.l_comoment`][lmo.l_comoment]
+        - [`lmo.l_ratio`][lmo.l_ratio]
 
-def tl_kurt(
-    a: AnyTensor,
-    /,
-    trim: Trimming = 1,
-    axis: int | None = None,
-    **kwargs: Any,
-) -> ScalarOrArray[np.float_]:
-    """
-    TL-kurtosis coefficient, $\\tau_4^{(t_1, t_2)}$; the 4th sample TL-moment
-    ratio.
     """
-    return tl_ratio(a, 4, trim=trim, axis=axis, **kwargs)
+    rs = np.stack(np.broadcast_arrays(np.asarray(r), np.asarray(s)))
+    L_r, L_s = l_comoment(a, rs, trim, rowvar=rowvar, dtype=dtype, **kwargs)
 
+    l_s = np.diagonal(L_s, axis1=-2, axis2=-1)
 
-# L-moment aliasses
+    return L_r / np.expand_dims(l_s, -1)
 
-def l_moment(
-    a: AnyTensor,
-    r: int,
+
+def l_coloc(
+    a: npt.ArrayLike,
     /,
-    axis: int | None = None,
+    trim: tuple[int, int] = (0, 0),
+    rowvar: bool = True,
+    dtype: np.dtype[T] | type[T] = np.float_,
     **kwargs: Any,
-) -> ScalarOrArray[np.float_]:
+) -> npt.NDArray[T]:
     """
-    The $r$-th sample L-moment, $\\lambda_r$.
-    Alias of [`lmo.tl_moment(..., trim=0)`][lmo.univariate.tl_moment].
+    L-colocation matrix of 1st L-comoment estimates, $\\Lambda^{(t_1, t_2)}_1$.
+
+    Alias for [`lmo.l_comoment(a, 1, *, **)`][lmo.l_comoment].
 
-    According to [Wikipedia](https://wikipedia.org/wiki/L-moment):
+    Notes:
+        If `trim = (0, 0)` (default), the L-colocation for $[ij]$ is the
+        L-location $\\lambda_1$ of $x_i$, independent of $x_j$.
 
-    > L-moments are far more meaningful when dealing with outliers in data
-    > than conventional moments.
+    Examples:
+        Without trimming, the L-colocation only provides marginal information:
 
-    Note that L-moments are robust to outliers, but not resistant to extreme
-    values.
+        >>> import lmo, numpy as np
+        >>> rng = np.random.default_rng(12345)
+        >>> x = rng.multivariate_normal([0, 0], [[6, -3], [-3, 3.5]], 99).T
+        >>> lmo.l_loc(x, axis=-1)
+        array([-0.02678225,  0.03008309])
+        >>> lmo.l_coloc(x)
+        array([[-0.02678225, -0.02678225],
+               [ 0.03008309,  0.03008309]])
+
+        But the trimmed L-locations are a different story...
+
+        >>> lmo.l_loc(x, trim=(1, 1), axis=-1)
+        array([-0.10488868, -0.00625729])
+        >>> lmo.l_coloc(x, trim=(1, 1))
+        array([[-0.10488868, -0.03797989],
+               [ 0.03325074, -0.00625729]])
 
-    Often the Method of L-moment (LMM) outperforms the conventional method of
-    moments (MM) and maximum likelihood estimation (MLE), e.g. ftting of the
-    ``scipy.stats.genextreme`` (generalized extreme value, GED) distribution.
+        What this tells us, is somehwat of a mystery: trimmed L-comoments have
+        been only been briefly *mentioned* once or twice in the literature.
 
 
     See Also:
-        - [J.R.M. Hosking (1990)](https://jstor.org/stable/2345653)
-        - [L-moment - Wikipedia](https://wikipedia.org/wiki/L-moment)
+        - [`lmo.l_comoment`][lmo.l_comoment]
+        - [`lmo.l_loc`][lmo.l_loc]
+        - [`numpy.mean`][numpy.mean]
 
     """
-    return tl_moment(a, r, trim=0, axis=axis, **kwargs)
+    return l_comoment(a, 1, trim, rowvar=rowvar, dtype=dtype, **kwargs)
 
 
-def l_ratio(
-    a: AnyTensor,
-    r: int,
+def l_coscale(
+    a: npt.ArrayLike,
     /,
-    k: int = 2,
-    axis: int | None = None,
+    trim: tuple[int, int] = (0, 0),
+    rowvar: bool = True,
+    dtype: np.dtype[T] | type[T] = np.float_,
     **kwargs: Any,
-) -> ScalarOrArray[np.float_]:
+) -> npt.NDArray[T]:
     """
-    Ratio of the r-th and k-th (2nd by default) sample L-moments:
+    L-coscale matrix of 2nd L-comoment estimates, $\\Lambda^{(t_1, t_2)}_2$.
 
-    $$
-    \\tau_{r, k} = \\frac{\\lambda_{r}}{\\lambda_{k}}
-    $$
+    Alias for [`lmo.l_comoment(a, 2, *, **)`][lmo.l_comoment].
 
-    Alias of [`lmo.tl_ratio(..., trim=0)`][lmo.univariate.tl_ratio].
+    Analogous to the (auto-) variance-covariance matrix, the L-coscale matrix
+    is positive semi-definite, and its main diagonal contains the L-scale's.
+    conversely, the L-coscale matrix is inherently assymmetric, thus yielding
+    more information.
 
-    Notes:
-        Tthe L-moment ratio's are bounded within the interval $[-1, 1)$.
+    Examples:
+        >>> import lmo, numpy as np
+        >>> rng = np.random.default_rng(12345)
+        >>> x = rng.multivariate_normal([0, 0], [[6, -3], [-3, 3.5]], 99).T
+        >>> lmo.l_scale(x, trim=(1, 1), axis=-1)
+        array([0.66698774, 0.54440895])
+        >>> lmo.l_coscale(x, trim=(1, 1))
+        array([[ 0.66698774, -0.41025416],
+               [-0.37918065,  0.54440895]])
+
+    See Also:
+        - [`lmo.l_comoment`][lmo.l_comoment]
+        - [`lmo.l_scale`][lmo.l_scale]
+        - [`numpy.cov`][numpy.cov]
 
     """
-    return tl_ratio(a, r, k, trim=0, axis=axis, **kwargs)
+    return l_comoment(a, 2, trim, rowvar=rowvar, dtype=dtype, **kwargs)
 
 
-def l_loc(
-    a: AnyTensor,
+def l_corr(
+    a: npt.ArrayLike,
     /,
-    axis: int | None = None,
+    trim: tuple[int, int] = (0, 0),
+    rowvar: bool = True,
+    dtype: np.dtype[T] | type[T] = np.float_,
     **kwargs: Any,
-) -> ScalarOrArray[np.float_]:
+) -> npt.NDArray[T]:
     """
-    L-location: the first sample L-moment.
-    Equivalent to [`lmo.tl_loc(a, 0, **kwargs)`][lmo.univariate.tl_loc].
+    Sample L-correlation coefficient matrix $\\tilde\\Lambda^{(t_1, t_2)}_2$;
+    the ratio of the L-coscale matrix over the L-scale **column**-vectors.
 
-    Notes:
-        The L-location is equivalent to the (arithmetic) sample mean.
+    Alias for [`lmo.l_coratio(a, 2, 2, *, **)`][lmo.l_coratio].
 
-    """
-    return l_moment(a, 1, axis=axis, **kwargs)
+    The diagonal consists of all 1's.
 
+    Where the pearson correlation coefficient measures linearity, the
+    (T)L-correlation coefficient measures monotonicity.
 
-def l_scale(
-    a: AnyTensor,
-    /,
-    axis: int | None = None,
-    **kwargs: Any,
-) -> ScalarOrArray[np.float_]:
-    """
-    L-scale: the second L-moment.
-    Equivalent to [`lmo.tl_scale(a, 0, **kwargs)`][lmo.univariate.tl_scale].
+    Examples:
+        >>> import lmo, numpy as np
+        >>> rng = np.random.default_rng(12345)
+        >>> cov = np.array([[6, -3], [-3, 3.5]])
+        >>> x = rng.multivariate_normal([0, 0], [[6, -3], [-3, 3.5]], 99).T
+        >>> lmo.l_corr(x)
+        array([[ 1.        , -0.65247355],
+               [-0.67503962,  1.        ]])
 
-    Notes:
-        The L-scale is equivalent to half the [mean absolute difference](
-        https://wikipedia.org/wiki/Mean_absolute_difference).
+        Let's compare this with the theoretical correlation
+
+        >>> cov[0, 1] / np.sqrt(cov[0, 0] * cov[1, 1])
+        -0.6546536707079772
+
+        and the (Pearson) correlation coefficient matrix:
+
+        >>> np.corrcoef(x)
+        array([[ 1.        , -0.66383285],
+               [-0.66383285,  1.        ]])
+
+
+
+    See Also:
+        - [`lmo.l_coratio`][lmo.l_coratio]
+        - [`numpy.corrcoef`][numpy.corrcoef]
 
     """
-    return l_moment(a, 2, axis=axis, **kwargs)
+    return l_coratio(a, 2, 2, trim, rowvar=rowvar, dtype=dtype, **kwargs)
 
 
-def l_skew(
-    a: AnyTensor,
+def l_coskew(
+    a: npt.ArrayLike,
     /,
-    axis: int | None = None,
+    trim: tuple[int, int] = (0, 0),
+    rowvar: bool = True,
+    dtype: np.dtype[T] | type[T] = np.float_,
     **kwargs: Any,
-) -> ScalarOrArray[np.float_]:
+) -> npt.NDArray[T]:
     """
-    L-skewness coefficient; the 3rd sample L-moment ratio.
-    Equivalent to [`lmo.tl_skew(a, 0, **kwargs)`][lmo.univariate.tl_skew].
+    Sample L-coskewness coefficient matrix $\\tilde\\Lambda^{(t_1, t_2)}_3$.
+
+    Alias for [`lmo.l_coratio(a, 3, 2, *, **)`][lmo.l_coratio].
+
+    See Also:
+        - [`lmo.l_coratio`][lmo.l_coratio]
+        - [`lmo.l_skew`][lmo.l_skew]
+
     """
-    return l_ratio(a, 3, axis=axis, **kwargs)
+    return l_coratio(a, 3, 2, trim, rowvar=rowvar, dtype=dtype, **kwargs)
 
 
-def l_kurt(
-    a: AnyTensor,
+def l_cokurtosis(
+    a: npt.ArrayLike,
     /,
-    axis: int | None = None,
+    trim: tuple[int, int] = (0, 0),
+    rowvar: bool = True,
+    dtype: np.dtype[T] | type[T] = np.float_,
     **kwargs: Any,
-) -> ScalarOrArray[np.float_]:
+) -> npt.NDArray[T]:
     """
-    L-kurtosis coefficient; the 4th sample L-moment ratio.
-    Equivalent to [`lmo.tl_kurt(a, 0, **kwargs)`][lmo.univariate.tl_kurt].
+    Sample L-cokurtosis coefficient matrix $\\tilde\\Lambda^{(t_1, t_2)}_4$.
 
-    Notes:
-        The L-kurtosis $\\tau_4$ lies within the interval
-        $[-\\frac{1}{4}, 1)$, and by the L-skewness $\\tau_3$ as
-        $5 \\tau_3^2 - 1 \\le 4 \\tau_4$.
+    Alias for [`lmo.l_coratio(a, 4, 2, *, **)`][lmo.l_coratio].
+
+    See Also:
+        - [`lmo.l_coratio`][lmo.l_coratio]
+        - [`lmo.l_kurtosis`][lmo.l_kurtosis]
 
     """
-    return l_ratio(a, 4, axis=axis, **kwargs)
+    return l_coratio(a, 4, 2, trim, rowvar=rowvar, dtype=dtype, **kwargs)
```

### Comparing `lmo-0.4.0/pyproject.toml` & `lmo-0.5.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "oldest-supported-numpy"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "lmo"
-version = "0.4.0"
+version = "0.5.0"
 description = "L-Moments for robust statistics."
 authors = ["Joren Hammudoglu <jhammudoglu@gmail.com>"]
 readme = "README.md"
 license = "BSD-3-Clause"
 homepage = "https://jorenham.github.io/lmo/"
 repository = "https://github.com/jorenham/lmo/"
 classifiers = [
@@ -25,52 +25,60 @@
 
 [tool.poetry.urls]
 Documentation = "https://jorenham.github.io/lmo/"
 "Bug Tracker" = "https://github.com/jorenham/lmo/issues"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-numpy = "^1.20"
+numpy = "^1.21"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3"
 hypothesis = {extras = ["numpy"], version = "^6.75"}
 pyright = "^1.1"
 ruff = ">=0.0.263,<1.0"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.4.3"
 mkdocs-material = ">=9.1.9"
 mkdocstrings = {extras = ["python"], version = ">=0.21.2,<1.0"}
 mkdocs-include-markdown-plugin = { version = ">=4.0.4", python = "<3.12" }
-mike = "^1.1.2"
+
 
 [tool.pytest.ini_options]
 minversion = "7.0"
-addopts = ["-ra", "-W error", "--showlocals", "--strict-markers", "--strict-config"]
-testpaths = ["tests"]
+addopts = [
+    "-ra",
+    "-W error",
+    "--showlocals",
+    "--strict-markers",
+    "--strict-config",
+    "--doctest-modules",
+]
+doctest_optionflags = ["NORMALIZE_WHITESPACE", "IGNORE_EXCEPTION_DETAIL"]
+
 
 [tool.pyright]
 include = ["lmo"]
 exclude = [
     "**/__pycache__",
     "**/.pytest_cache",
     ".git",
     ".github",
     ".hypothesis",
     ".pytest_cache",
     ".ruff_cache",
-    ".venv",
     "dist",
     "docs",
 ]
 venvPath = ".venv"
 pythonVersion = "3.10"
 pythonPlatform = "Linux"
 typeCheckingMode = "strict"
 
+
 [tool.ruff]
 line-length = 80
 target-version = "py310"
 
 [tool.ruff.pydocstyle]
 convention = "google"
```

### Comparing `lmo-0.4.0/PKG-INFO` & `lmo-0.5.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmo
-Version: 0.4.0
+Version: 0.5.0
 Summary: L-Moments for robust statistics.
 Home-page: https://jorenham.github.io/lmo/
 License: BSD-3-Clause
 Author: Joren Hammudoglu
 Author-email: jhammudoglu@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -16,15 +16,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
-Requires-Dist: numpy (>=1.20,<2.0)
+Requires-Dist: numpy (>=1.21,<2.0)
 Project-URL: Bug Tracker, https://github.com/jorenham/lmo/issues
 Project-URL: Documentation, https://jorenham.github.io/lmo/
 Project-URL: Repository, https://github.com/jorenham/lmo/
 Description-Content-Type: text/markdown
 
 <!--head-start-->
 
@@ -34,20 +34,14 @@
 
 ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/jorenham/lmo/CI.yml?branch=master&style=flat-square)
 [![PyPI](https://img.shields.io/pypi/v/lmo?style=flat-square)](https://pypi.org/project/lmo/)
 [![versions](https://img.shields.io/pypi/pyversions/lmo?style=flat-square)](https://github.com/jorenham/lmo)
 [![license](https://img.shields.io/github/license/jorenham/lmo?style=flat-square)](https://github.com/jorenham/lmo/blob/master/LICENSE?)
 
 
-Streamlined calculation of L-moments and TL-moments.
+Generalized trimmed **L-mo**ments for robust statistics. 
 
 ---
 <!--head-end-->
 
-[Documentation](https://jorenham.github.io/lmo/)
-
----
-
-*Examples coming soon*.
-
-
+See the [documentation](https://jorenham.github.io/lmo/) for usage examples and code reference.
```

