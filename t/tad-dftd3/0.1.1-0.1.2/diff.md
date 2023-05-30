# Comparing `tmp/tad_dftd3-0.1.1.tar.gz` & `tmp/tad_dftd3-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tad_dftd3-0.1.1.tar", last modified: Wed May 17 06:06:17 2023, max compression
+gzip compressed data, was "tad_dftd3-0.1.2.tar", last modified: Tue May 30 06:48:13 2023, max compression
```

## Comparing `tad_dftd3-0.1.1.tar` & `tad_dftd3-0.1.2.tar`

### file list

```diff
@@ -1,36 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:06:17.512986 tad_dftd3-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-17 06:06:10.000000 tad_dftd3-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10231 2023-05-17 06:06:17.512986 tad_dftd3-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9443 2023-05-17 06:06:10.000000 tad_dftd3-0.1.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-17 06:06:10.000000 tad_dftd3-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-17 06:06:17.512986 tad_dftd3-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-17 06:06:10.000000 tad_dftd3-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:06:17.504986 tad_dftd3-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:06:17.508986 tad_dftd3-0.1.1/src/tad_dftd3/
--rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-05-17 06:06:10.000000 tad_dftd3-0.1.1/src/tad_dftd3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-17 06:06:10.000000 tad_dftd3-0.1.1/src/tad_dftd3/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:06:17.508986 tad_dftd3-0.1.1/src/tad_dftd3/damping/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-17 06:06:10.000000 tad_dftd3-0.1.1/src/tad_dftd3/damping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-05-17 06:06:10.000000 tad_dftd3-0.1.1/src/tad_dftd3/damping/atm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-17 06:06:10.000000 tad_dftd3-0.1.1/src/tad_dftd3/damping/rational.py
--rw-r--r--   0 runner    (1001) docker     (123)    75725 2023-05-17 06:06:10.000000 tad_dftd3-0.1.1/src/tad_dftd3/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-17 06:06:10.000000 tad_dftd3-0.1.1/src/tad_dftd3/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-05-17 06:06:10.000000 tad_dftd3-0.1.1/src/tad_dftd3/disp.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-17 06:06:10.000000 tad_dftd3-0.1.1/src/tad_dftd3/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-05-17 06:06:10.000000 tad_dftd3-0.1.1/src/tad_dftd3/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-05-17 06:06:10.000000 tad_dftd3-0.1.1/src/tad_dftd3/ncoord.py
--rw-r--r--   0 runner    (1001) docker     (123)    11702 2023-05-17 06:06:10.000000 tad_dftd3-0.1.1/src/tad_dftd3/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-17 06:06:10.000000 tad_dftd3-0.1.1/src/tad_dftd3/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-05-17 06:06:10.000000 tad_dftd3-0.1.1/src/tad_dftd3/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:06:17.508986 tad_dftd3-0.1.1/src/tad_dftd3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10231 2023-05-17 06:06:17.000000 tad_dftd3-0.1.1/src/tad_dftd3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-17 06:06:17.000000 tad_dftd3-0.1.1/src/tad_dftd3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 06:06:17.000000 tad_dftd3-0.1.1/src/tad_dftd3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-17 06:06:17.000000 tad_dftd3-0.1.1/src/tad_dftd3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-17 06:06:17.000000 tad_dftd3-0.1.1/src/tad_dftd3.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:06:17.512986 tad_dftd3-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-05-17 06:06:10.000000 tad_dftd3-0.1.1/tests/test_dftd3.py
--rw-r--r--   0 runner    (1001) docker     (123)     6894 2023-05-17 06:06:10.000000 tad_dftd3-0.1.1/tests/test_disp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-05-17 06:06:10.000000 tad_dftd3-0.1.1/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-05-17 06:06:10.000000 tad_dftd3-0.1.1/tests/test_ncoord.py
--rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-05-17 06:06:10.000000 tad_dftd3-0.1.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:48:13.358463 tad_dftd3-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-30 06:48:02.000000 tad_dftd3-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10231 2023-05-30 06:48:13.358463 tad_dftd3-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9443 2023-05-30 06:48:02.000000 tad_dftd3-0.1.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-30 06:48:02.000000 tad_dftd3-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-30 06:48:13.358463 tad_dftd3-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-30 06:48:02.000000 tad_dftd3-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:48:13.350463 tad_dftd3-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:48:13.358463 tad_dftd3-0.1.2/src/tad_dftd3/
+-rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-05-30 06:48:02.000000 tad_dftd3-0.1.2/src/tad_dftd3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-30 06:48:02.000000 tad_dftd3-0.1.2/src/tad_dftd3/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-30 06:48:02.000000 tad_dftd3-0.1.2/src/tad_dftd3/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:48:13.358463 tad_dftd3-0.1.2/src/tad_dftd3/damping/
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-30 06:48:02.000000 tad_dftd3-0.1.2/src/tad_dftd3/damping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-05-30 06:48:02.000000 tad_dftd3-0.1.2/src/tad_dftd3/damping/atm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-05-30 06:48:02.000000 tad_dftd3-0.1.2/src/tad_dftd3/damping/rational.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75725 2023-05-30 06:48:02.000000 tad_dftd3-0.1.2/src/tad_dftd3/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-30 06:48:02.000000 tad_dftd3-0.1.2/src/tad_dftd3/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7610 2023-05-30 06:48:02.000000 tad_dftd3-0.1.2/src/tad_dftd3/disp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-30 06:48:02.000000 tad_dftd3-0.1.2/src/tad_dftd3/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-05-30 06:48:02.000000 tad_dftd3-0.1.2/src/tad_dftd3/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-05-30 06:48:02.000000 tad_dftd3-0.1.2/src/tad_dftd3/ncoord.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 06:48:02.000000 tad_dftd3-0.1.2/src/tad_dftd3/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   893128 2023-05-30 06:48:02.000000 tad_dftd3-0.1.2/src/tad_dftd3/reference-c6.npy
+-rw-r--r--   0 runner    (1001) docker     (123)    12169 2023-05-30 06:48:02.000000 tad_dftd3-0.1.2/src/tad_dftd3/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-05-30 06:48:02.000000 tad_dftd3-0.1.2/src/tad_dftd3/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-05-30 06:48:02.000000 tad_dftd3-0.1.2/src/tad_dftd3/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:48:13.358463 tad_dftd3-0.1.2/src/tad_dftd3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10231 2023-05-30 06:48:13.000000 tad_dftd3-0.1.2/src/tad_dftd3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-30 06:48:13.000000 tad_dftd3-0.1.2/src/tad_dftd3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 06:48:13.000000 tad_dftd3-0.1.2/src/tad_dftd3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-30 06:48:13.000000 tad_dftd3-0.1.2/src/tad_dftd3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-30 06:48:13.000000 tad_dftd3-0.1.2/src/tad_dftd3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:48:13.358463 tad_dftd3-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-05-30 06:48:02.000000 tad_dftd3-0.1.2/tests/test_dftd3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-05-30 06:48:02.000000 tad_dftd3-0.1.2/tests/test_disp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-05-30 06:48:02.000000 tad_dftd3-0.1.2/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-05-30 06:48:02.000000 tad_dftd3-0.1.2/tests/test_ncoord.py
```

### Comparing `tad_dftd3-0.1.1/LICENSE` & `tad_dftd3-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.1.1/PKG-INFO` & `tad_dftd3-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tad_dftd3
-Version: 0.1.1
+Version: 0.1.2
 Summary: Torch autodiff DFT-D3 implementation
 License: Apache-2.0
 Project-URL: Documentation, https://tad-dftd3.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/dftd3/tad-dftd3
 Project-URL: Tracker, https://github.com/dftd3/tad-dftd3/issues
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tad_dftd3-0.1.1/README.rst` & `tad_dftd3-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.1.1/setup.cfg` & `tad_dftd3-0.1.2/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tad_dftd3
-version = 0.1.1
+version = attr: tad_dftd3.__version__.__version__
 description = Torch autodiff DFT-D3 implementation
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 license = Apache-2.0
 license_files = LICENSE
 classifiers = 
 	License :: OSI Approved :: Apache Software License
@@ -41,15 +41,15 @@
 	pre-commit
 	pylint
 	pytest
 	pytest-random-order
 	tox
 
 [options.package_data]
-dxtb = 
+tad_dftd3 = 
 	py.typed
-	src/*/*.npy
+	*.npy
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `tad_dftd3-0.1.1/src/tad_dftd3/__init__.py` & `tad_dftd3-0.1.2/src/tad_dftd3/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -71,14 +71,15 @@
 >>> print(energy[0] - 2*energy[1])
 tensor(-0.0034288)
 """
 import torch
 
 from . import damping, data, disp, model, ncoord, reference, util
 from .typing import (
+    DD,
     CountingFunction,
     DampingFunction,
     Dict,
     Optional,
     Tensor,
     WeightingFunction,
 )
@@ -89,14 +90,15 @@
     positions: Tensor,
     param: Dict[str, Tensor],
     *,
     ref: Optional[reference.Reference] = None,
     rcov: Optional[Tensor] = None,
     rvdw: Optional[Tensor] = None,
     r4r2: Optional[Tensor] = None,
+    cutoff: Optional[Tensor] = None,
     counting_function: CountingFunction = ncoord.exp_count,
     weighting_function: WeightingFunction = model.gaussian_weight,
     damping_function: DampingFunction = damping.rational_damping,
 ) -> Tensor:
     """
     Evaluate DFT-D3 dispersion energy for a batch of geometries.
 
@@ -121,20 +123,23 @@
     weighting_function : Callable, optional
         Function to calculate weight of individual reference systems.
     counting_function : Callable, optional
         Calculates counting value in range 0 to 1 for each atom pair.
 
     Returns
     -------
-    torch.Tensor
-        DFT-D3 dispersion energy for each geometry.
+    Tensor
+        Atom-resolved DFT-D3 dispersion energy for each geometry.
     """
+    dd: DD = {"device": positions.device, "dtype": positions.dtype}
 
+    if cutoff is None:
+        cutoff = torch.tensor(50.0, **dd)
     if ref is None:
-        ref = reference.Reference().type(positions.dtype).to(positions.device)
+        ref = reference.Reference(**dd)
     if rcov is None:
         rcov = data.covalent_rad_d3[numbers].type(positions.dtype).to(positions.device)
     if rvdw is None:
         rvdw = (
             data.vdw_rad_d3[numbers.unsqueeze(-1), numbers.unsqueeze(-2)]
             .type(positions.dtype)
             .to(positions.device)
@@ -151,10 +156,11 @@
         numbers,
         positions,
         param,
         c6,
         rvdw,
         r4r2,
         damping_function,
+        cutoff=cutoff,
     )
 
     return energy
```

### Comparing `tad_dftd3-0.1.1/src/tad_dftd3/constants.py` & `tad_dftd3-0.1.2/src/tad_dftd3/constants.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.1.1/src/tad_dftd3/damping/atm.py` & `tad_dftd3-0.1.2/src/tad_dftd3/damping/atm.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+# This file is part of tad-dftd3.
+# SPDX-Identifier: Apache-2.0
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 r"""
 Axilrod-Teller-Muto (ATM) dispersion term
 =========================================
 
 This module provides the dispersion energy evaluation for the three-body
 Axilrod-Teller-Muto dispersion term.
 
@@ -15,16 +29,16 @@
     {\left(r_\text{AB} r_\text{BC} r_\text{AC} \right)^3} \\
     f_\text{damp} &=
     \dfrac{1}{1+ 6 \left(\overline{R}_\text{ABC}\right)^{-16}}
 """
 import torch
 
 from .. import defaults
-from ..typing import Tensor
-from ..util import real_pairs, real_triples
+from ..typing import DD, Tensor
+from ..util import cdist, real_pairs, real_triples
 
 
 def dispersion_atm(
     numbers: Tensor,
     positions: Tensor,
     c6: Tensor,
     rvdw: Tensor,
@@ -56,61 +70,64 @@
         Exponent of zero damping function. Defaults to `14.0`.
 
     Returns
     -------
     Tensor
         Atom-resolved ATM dispersion energy.
     """
-    dd = {"device": positions.device, "dtype": positions.dtype}
+    dd: DD = {"device": positions.device, "dtype": positions.dtype}
 
     s9 = s9.type(positions.dtype).to(positions.device)
     rs9 = rs9.type(positions.dtype).to(positions.device)
     alp = alp.type(positions.dtype).to(positions.device)
 
     cutoff2 = cutoff * cutoff
     srvdw = rs9 * rvdw
 
+    mask_pairs = real_pairs(numbers, diagonal=False)
+    mask_triples = real_triples(numbers, diagonal=False)
+
+    eps = torch.tensor(torch.finfo(positions.dtype).eps, **dd)
+
     # C9_ABC = s9 * sqrt(|C6_AB * C6_AC * C6_BC|)
     c9 = s9 * torch.sqrt(
-        torch.abs(c6.unsqueeze(-1) * c6.unsqueeze(-2) * c6.unsqueeze(-3))
+        torch.clamp(
+            torch.abs(c6.unsqueeze(-1) * c6.unsqueeze(-2) * c6.unsqueeze(-3)), min=eps
+        )
     )
 
     r0ij = srvdw.unsqueeze(-1)
     r0ik = srvdw.unsqueeze(-2)
     r0jk = srvdw.unsqueeze(-3)
     r0 = r0ij * r0ik * r0jk
 
     # actually faster than other alternatives
     # very slow: (pos.unsqueeze(-2) - pos.unsqueeze(-3)).pow(2).sum(-1)
     distances = torch.pow(
         torch.where(
-            real_pairs(numbers, diagonal=False),
-            torch.cdist(
-                positions, positions, p=2, compute_mode="use_mm_for_euclid_dist"
-            ),
-            torch.tensor(torch.finfo(positions.dtype).eps, **dd),
+            mask_pairs,
+            cdist(positions, positions, p=2),
+            eps,
         ),
         2.0,
     )
 
     r2ij = distances.unsqueeze(-1)
     r2ik = distances.unsqueeze(-2)
     r2jk = distances.unsqueeze(-3)
     r2 = r2ij * r2ik * r2jk
     r1 = torch.sqrt(r2)
-    r3 = r1 * r2
-    r5 = r2 * r3
+    # add epsilon to avoid zero division later
+    r3 = torch.where(mask_triples, r1 * r2, eps)
+    r5 = torch.where(mask_triples, r2 * r3, eps)
 
     fdamp = 1.0 / (1.0 + 6.0 * (r0 / r1) ** ((alp + 2.0) / 3.0))
 
     s = (r2ij + r2jk - r2ik) * (r2ij - r2jk + r2ik) * (-r2ij + r2jk + r2ik)
     ang = torch.where(
-        real_triples(numbers, diagonal=False)
-        * (r2ij <= cutoff2)
-        * (r2jk <= cutoff2)
-        * (r2jk <= cutoff2),
+        mask_triples * (r2ij <= cutoff2) * (r2jk <= cutoff2) * (r2jk <= cutoff2),
         0.375 * s / r5 + 1.0 / r3,
         torch.tensor(0.0, **dd),
     )
 
     energy = ang * fdamp * c9
     return torch.sum(energy, dim=(-2, -1)) / 6.0
```

### Comparing `tad_dftd3-0.1.1/src/tad_dftd3/data.py` & `tad_dftd3-0.1.2/src/tad_dftd3/data.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.1.1/src/tad_dftd3/disp.py` & `tad_dftd3-0.1.2/src/tad_dftd3/disp.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,16 +52,16 @@
 >>> print(torch.sum(energy[0] - energy[1] - energy[2]))  # energy in Hartree
 tensor(-0.0003964)
 """
 import torch
 
 from . import data, defaults
 from .damping import dispersion_atm, rational_damping
-from .typing import Any, DampingFunction, Dict, Optional, Tensor
-from .util import real_pairs
+from .typing import DD, Any, DampingFunction, Dict, Optional, Tensor
+from .util import cdist, real_pairs
 
 
 def dispersion(
     numbers: Tensor,
     positions: Tensor,
     param: Dict[str, Tensor],
     c6: Tensor,
@@ -87,16 +87,21 @@
     rvdw : Tensor
         Van der Waals radii of the atoms in the system.
     r4r2 : Tensor
         r⁴ over r² expectation values of the atoms in the system.
     damping_function : Callable
         Damping function evaluate distance dependent contributions.
         Additional arguments are passed through to the function.
+
+    Returns
+    -------
+    Tensor
+        Atom-resolved DFT-D3 dispersion energy for each geometry.
     """
-    dd = {"device": positions.device, "dtype": positions.dtype}
+    dd: DD = {"device": positions.device, "dtype": positions.dtype}
 
     if cutoff is None:
         cutoff = torch.tensor(50.0, **dd)
     if r4r2 is None:
         r4r2 = (
             data.sqrt_z_r4_over_r2[numbers].type(positions.dtype).to(positions.device)
         )
@@ -153,20 +158,20 @@
         Atomic C6 dispersion coefficients.
     r4r2 : Tensor
         r⁴ over r² expectation values of the atoms in the system.
     damping_function : Callable
         Damping function evaluate distance dependent contributions.
         Additional arguments are passed through to the function.
     """
-    dd = {"device": positions.device, "dtype": positions.dtype}
+    dd: DD = {"device": positions.device, "dtype": positions.dtype}
 
     mask = real_pairs(numbers, diagonal=False)
     distances = torch.where(
         mask,
-        torch.cdist(positions, positions, p=2, compute_mode="use_mm_for_euclid_dist"),
+        cdist(positions, positions, p=2),
         torch.tensor(torch.finfo(positions.dtype).eps, **dd),
     )
 
     qq = 3 * r4r2.unsqueeze(-1) * r4r2.unsqueeze(-2)
     c8 = c6 * qq
 
     t6 = torch.where(
@@ -220,14 +225,14 @@
         Scaling for van-der-Waals radii in damping function. Defaults to `4.0/3.0`.
 
     Returns
     -------
     Tensor
         Atom-resolved three-body dispersion energy.
     """
-    dd = {"device": positions.device, "dtype": positions.dtype}
+    dd: DD = {"device": positions.device, "dtype": positions.dtype}
 
     alp = param.get("alp", torch.tensor(14.0, **dd))
     s9 = param.get("s9", torch.tensor(1.0, **dd))
     rs9 = rs9.type(positions.dtype).to(positions.device)
 
     return dispersion_atm(numbers, positions, c6, rvdw, cutoff, s9, rs9, alp)
```

### Comparing `tad_dftd3-0.1.1/src/tad_dftd3/exception.py` & `tad_dftd3-0.1.2/src/tad_dftd3/exception.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.1.1/src/tad_dftd3/ncoord.py` & `tad_dftd3-0.1.2/src/tad_dftd3/ncoord.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,16 +57,16 @@
 tensor([[2.9901006, 0.9977214, 0.9977214, 0.9977214, 0.0000000, 0.0000000],
         [3.0059586, 1.0318390, 3.0268824, 1.0061584, 1.0036336, 0.9989871],
         [3.0093639, 2.0046251, 1.0187057, 0.9978270, 1.0069743, 0.0000000]])
 """
 import torch
 
 from . import data
-from .typing import Any, CountingFunction, Optional, Tensor
-from .util import real_pairs
+from .typing import DD, Any, CountingFunction, Optional, Tensor
+from .util import cdist, real_pairs
 
 
 def exp_count(r: Tensor, r0: Tensor, kcn: float = 16.0) -> Tensor:
     """
     Exponential counting function for coordination number contributions.
 
     Parameters
@@ -112,15 +112,15 @@
     cutoff : float
         Real-space cutoff for the evaluation of counting function
 
     Returns
     -------
         Tensor: The coordination number of each atom in the system.
     """
-    dd = {"device": positions.device, "dtype": positions.dtype}
+    dd: DD = {"device": positions.device, "dtype": positions.dtype}
 
     if cutoff is None:
         cutoff = torch.tensor(25.0, **dd)
     if rcov is None:
         rcov = data.covalent_rad_d3[numbers].type(positions.dtype).to(positions.device)
     if numbers.shape != rcov.shape:
         raise ValueError(
@@ -128,15 +128,15 @@
         )
     if numbers.shape != positions.shape[:-1]:
         raise ValueError("Shape of positions is not consistent with atomic numbers")
 
     mask = real_pairs(numbers, diagonal=False)
     distances = torch.where(
         mask,
-        torch.cdist(positions, positions, p=2, compute_mode="use_mm_for_euclid_dist"),
+        cdist(positions, positions, p=2),
         torch.tensor(torch.finfo(positions.dtype).eps, **dd),
     )
 
     rc = rcov.unsqueeze(-2) + rcov.unsqueeze(-1)
     cf = torch.where(
         mask * (distances <= cutoff),
         counting_function(distances, rc.type(distances.dtype), **kwargs),
```

### Comparing `tad_dftd3-0.1.1/src/tad_dftd3/reference.py` & `tad_dftd3-0.1.2/src/tad_dftd3/reference.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,17 @@
 import os.path as op
 
 import torch
 
 from .typing import Any, NoReturn, Optional, Tensor
 
 
-def _load_cn(dtype: torch.dtype = torch.float) -> Tensor:
+def _load_cn(
+    dtype: torch.dtype = torch.float, device: Optional[torch.device] = None
+) -> Tensor:
     return torch.tensor(
         [
             [-1.0000, -1.0000, -1.0000, -1.0000, -1.0000],  # None
             [+0.9118, +0.0000, -1.0000, -1.0000, -1.0000],  # H
             [+0.0000, -1.0000, -1.0000, -1.0000, -1.0000],  # He
             [+0.0000, +0.9865, -1.0000, -1.0000, -1.0000],  # Li
             [+0.0000, +0.9808, +1.9697, -1.0000, -1.0000],  # Be
@@ -120,35 +122,40 @@
             [+0.0000, +0.9662, +1.8075, -1.0000, -1.0000],  # Ra
             [+0.0000, +2.9070, -1.0000, -1.0000, -1.0000],  # Ac
             [+0.0000, +2.8844, -1.0000, -1.0000, -1.0000],  # Th
             [+0.0000, +2.8738, -1.0000, -1.0000, -1.0000],  # Pa
             [+0.0000, +2.8878, -1.0000, -1.0000, -1.0000],  # U
             [+0.0000, +2.9095, -1.0000, -1.0000, -1.0000],  # Np
             [+0.0000, +1.9209, -1.0000, -1.0000, -1.0000],  # Pu
-        ]
-    ).type(dtype)
+        ],
+        device=device,
+        dtype=dtype,
+    )
 
 
-def _load_c6(dtype: torch.dtype = torch.float) -> Tensor:
+def _load_c6(
+    dtype: torch.dtype = torch.float, device: Optional[torch.device] = None
+) -> Tensor:
     """
     Load reference C6 coefficients from file and fill them into a tensor
     """
 
     # pylint: disable=import-outside-toplevel
     import math
 
     import numpy as np
 
-    ref = torch.from_numpy(
-        np.load(op.join(op.dirname(__file__), "reference-c6.npy"))
-    ).type(dtype)
+    path = op.join(op.dirname(__file__), "reference-c6.npy")
+    ref = torch.from_numpy(np.load(path)).type(dtype).to(device)
 
     n_element = (math.isqrt(8 * ref.shape[0] + 1) - 1) // 2 + 1
     n_reference = ref.shape[-1]
-    c6 = torch.zeros((n_element, n_element, n_reference, n_reference), dtype=dtype)
+    c6 = torch.zeros(
+        (n_element, n_element, n_reference, n_reference), dtype=dtype, device=device
+    )
 
     for i in range(1, n_element):
         for j in range(1, n_element):
             ij = i * (i - 1) // 2 + j - 1 if j < i else j * (j - 1) // 2 + i - 1
             c6[i, j, :, :] = ref[ij, :, :].T if j < i else ref[ij, :, :]
 
     return c6
@@ -172,20 +179,28 @@
         "__device",
     ]
 
     def __init__(
         self,
         cn: Optional[Tensor] = None,
         c6: Optional[Tensor] = None,
+        device: Optional[torch.device] = None,
+        dtype: Optional[torch.dtype] = None,
     ):
         if cn is None:
-            cn = _load_cn()
+            cn = _load_cn(
+                dtype if dtype is not None else torch.float,
+                device=device,
+            )
         self.cn = cn
         if c6 is None:
-            c6 = _load_c6()
+            c6 = _load_c6(
+                dtype if dtype is not None else torch.float,
+                device=device,
+            )
         self.c6 = c6
 
         self.__dtype = self.c6.dtype
         self.__device = self.c6.device
 
         if any(tensor.device != self.device for tensor in (self.cn, self.c6)):
             raise RuntimeError("All tensors must be on the same device!")
```

### Comparing `tad_dftd3-0.1.1/src/tad_dftd3/typing.py` & `tad_dftd3-0.1.2/src/tad_dftd3/typing.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,7 +45,17 @@
     """Representation of fundamental molecular structure (atom types and postions)."""
 
     numbers: Tensor
     """Tensor of atomic numbers"""
 
     positions: Tensor
     """Tensor of 3D coordinates of shape (n, 3)"""
+
+
+class DD(TypedDict):
+    """Collection of torch.device and torch.dtype."""
+
+    device: Union[torch.device, None]
+    """Device on which a tensor lives."""
+
+    dtype: torch.dtype
+    """Floating point precision of a tensor."""
```

### Comparing `tad_dftd3-0.1.1/src/tad_dftd3.egg-info/PKG-INFO` & `tad_dftd3-0.1.2/src/tad_dftd3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tad-dftd3
-Version: 0.1.1
+Version: 0.1.2
 Summary: Torch autodiff DFT-D3 implementation
 License: Apache-2.0
 Project-URL: Documentation, https://tad-dftd3.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/dftd3/tad-dftd3
 Project-URL: Tracker, https://github.com/dftd3/tad-dftd3/issues
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tad_dftd3-0.1.1/tests/test_disp.py` & `tad_dftd3-0.1.2/tests/test_disp.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,22 +51,24 @@
     sample = samples["PbH4-BiH3"]
     numbers = sample["numbers"]
     positions = sample["positions"].type(dtype)
     ref = sample["disp2"].type(dtype)
     c6 = sample["c6"].type(dtype)
     rvdw = data.vdw_rad_d3[numbers.unsqueeze(-1), numbers.unsqueeze(-2)]
     r4r2 = data.sqrt_z_r4_over_r2[numbers]
+    cutoff = torch.tensor(50.0, dtype=dtype)
+
     param = {
         "a1": positions.new_tensor(0.49484001),
         "s8": positions.new_tensor(0.78981345),
         "a2": positions.new_tensor(5.73083694),
     }
 
     energy = disp.dispersion(
-        numbers, positions, param, c6, rvdw, r4r2, disp.rational_damping
+        numbers, positions, param, c6, rvdw, r4r2, disp.rational_damping, cutoff=cutoff
     )
 
     assert energy.dtype == dtype
     assert pytest.approx(energy) == ref
 
 
 @pytest.mark.parametrize("dtype", [torch.float32, torch.float64])
@@ -93,25 +95,21 @@
     ref = util.pack(
         (
             sample1["disp2"].type(dtype),
             sample2["disp2"].type(dtype),
         )
     )
 
-    rvdw = data.vdw_rad_d3[numbers.unsqueeze(-1), numbers.unsqueeze(-2)]
-    r4r2 = data.sqrt_z_r4_over_r2[numbers]
     param = {
         "a1": positions.new_tensor(0.49484001),
         "s8": positions.new_tensor(0.78981345),
         "a2": positions.new_tensor(5.73083694),
     }
 
-    energy = disp.dispersion(
-        numbers, positions, param, c6, rvdw, r4r2, disp.rational_damping
-    )
+    energy = disp.dispersion(numbers, positions, param, c6)
 
     assert energy.dtype == dtype
     assert pytest.approx(energy) == ref
 
 
 @pytest.mark.parametrize("dtype", [torch.float, torch.double])
 @pytest.mark.parametrize("name", ["SiH4", "MB16_43_01"])
```

### Comparing `tad_dftd3-0.1.1/tests/test_model.py` & `tad_dftd3-0.1.2/tests/test_model.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,51 +11,61 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
 Test model parameters.
 """
+from math import sqrt
 
 import pytest
 import torch
 
 from tad_dftd3 import model, reference, util
 
 from .samples import samples
 from .utils import get_device_from_str
 
+sample_list = ["SiH4", "PbH4-BiH3", "C6H5I-CH3SH", "MB16_43_01"]
+
 
 @pytest.mark.parametrize("dtype", [torch.float32, torch.float64])
-def test_gw_single(dtype: torch.dtype) -> None:
-    sample = samples["PbH4-BiH3"]
+@pytest.mark.parametrize("name", sample_list)
+def test_gw_single(dtype: torch.dtype, name: str) -> None:
+    tol = sqrt(torch.finfo(dtype).eps)
+
+    sample = samples[name]
     numbers = sample["numbers"]
-    ref = reference.Reference().type(dtype)
+    ref = reference.Reference(dtype=dtype)
     cn = sample["cn"].type(dtype)
     refgw = sample["weights"].type(dtype)
 
     weights = model.weight_references(numbers, cn, ref, model.gaussian_weight)
 
     assert weights.dtype == dtype
-    assert pytest.approx(weights) == refgw
+    assert pytest.approx(refgw, abs=tol, rel=tol) == weights
 
 
 @pytest.mark.parametrize("dtype", [torch.float32, torch.float64])
-def test_gw_batch(dtype: torch.dtype) -> None:
+@pytest.mark.parametrize("name1", ["SiH4"])
+@pytest.mark.parametrize("name2", sample_list)
+def test_gw_batch(dtype: torch.dtype, name1: str, name2: str) -> None:
+    tol = sqrt(torch.finfo(dtype).eps)
+
     sample1, sample2 = (
-        samples["PbH4-BiH3"],
-        samples["C6H5I-CH3SH"],
+        samples[name1],
+        samples[name2],
     )
     numbers = util.pack(
         (
             sample1["numbers"],
             sample2["numbers"],
         )
     )
-    ref = reference.Reference().type(dtype)
+    ref = reference.Reference(dtype=dtype)
     cn = util.pack(
         (
             sample1["cn"].type(dtype),
             sample2["cn"].type(dtype),
         )
     )
     refgw = util.pack(
@@ -64,44 +74,51 @@
             sample2["weights"].type(dtype),
         )
     )
 
     weights = model.weight_references(numbers, cn, ref, model.gaussian_weight)
 
     assert weights.dtype == dtype
-    assert pytest.approx(weights) == refgw
+    assert pytest.approx(refgw, abs=tol, rel=tol) == weights
 
 
 @pytest.mark.parametrize("dtype", [torch.float32, torch.float64])
-def test_c6_single(dtype: torch.dtype) -> None:
-    sample = samples["PbH4-BiH3"]
+@pytest.mark.parametrize("name", sample_list)
+def test_c6_single(dtype: torch.dtype, name: str) -> None:
+    tol = sqrt(torch.finfo(dtype).eps)
+
+    sample = samples[name]
     numbers = sample["numbers"]
-    ref = reference.Reference().type(dtype)
+    ref = reference.Reference(dtype=dtype)
     weights = sample["weights"].type(dtype)
     refc6 = sample["c6"].type(dtype)
 
     c6 = model.atomic_c6(numbers, weights, ref)
 
     assert c6.dtype == dtype
-    assert pytest.approx(c6) == refc6
+    assert pytest.approx(refc6, abs=tol, rel=tol) == c6
 
 
 @pytest.mark.parametrize("dtype", [torch.float32, torch.float64])
-def test_c6_batch(dtype: torch.dtype) -> None:
+@pytest.mark.parametrize("name1", ["SiH4"])
+@pytest.mark.parametrize("name2", sample_list)
+def test_c6_batch(dtype: torch.dtype, name1: str, name2: str) -> None:
+    tol = sqrt(torch.finfo(dtype).eps)
+
     sample1, sample2 = (
-        samples["PbH4-BiH3"],
-        samples["C6H5I-CH3SH"],
+        samples[name1],
+        samples[name2],
     )
     numbers = util.pack(
         (
             sample1["numbers"],
             sample2["numbers"],
         )
     )
-    ref = reference.Reference().type(dtype)
+    ref = reference.Reference(dtype=dtype)
     weights = util.pack(
         (
             sample1["weights"].type(dtype),
             sample2["weights"].type(dtype),
         )
     )
     refc6 = util.pack(
@@ -110,15 +127,15 @@
             sample2["c6"].type(dtype),
         )
     )
 
     c6 = model.atomic_c6(numbers, weights, ref)
 
     assert c6.dtype == dtype
-    assert pytest.approx(c6) == refc6
+    assert pytest.approx(refc6, abs=tol, rel=tol) == c6
 
 
 @pytest.mark.parametrize("dtype", [torch.float32, torch.float64])
 def test_reference_dtype(dtype: torch.dtype) -> None:
     ref = reference.Reference().type(dtype)
     assert ref.dtype == dtype
```

### Comparing `tad_dftd3-0.1.1/tests/test_ncoord.py` & `tad_dftd3-0.1.2/tests/test_ncoord.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,18 +39,21 @@
 
 
 @pytest.mark.parametrize("dtype", [torch.float32, torch.float64])
 def test_cn_single(dtype: torch.dtype) -> None:
     sample = samples["PbH4-BiH3"]
     numbers = sample["numbers"]
     positions = sample["positions"].type(dtype)
+    cutoff = torch.tensor(25, dtype=dtype)
     ref = sample["cn"].type(dtype)
 
     rcov = data.covalent_rad_d3[numbers]
-    cn = ncoord.coordination_number(numbers, positions, rcov, ncoord.exp_count)
+    cn = ncoord.coordination_number(
+        numbers, positions, rcov, ncoord.exp_count, cutoff=cutoff
+    )
     assert cn.dtype == dtype
     assert pytest.approx(cn) == ref
 
 
 @pytest.mark.parametrize("dtype", [torch.float32, torch.float64])
 def test_cn_batch(dtype: torch.dtype) -> None:
     sample1, sample2 = (
@@ -72,11 +75,10 @@
     ref = util.pack(
         (
             sample1["cn"].type(dtype),
             sample2["cn"].type(dtype),
         )
     )
 
-    rcov = data.covalent_rad_d3[numbers]
-    cn = ncoord.coordination_number(numbers, positions, rcov, ncoord.exp_count)
+    cn = ncoord.coordination_number(numbers, positions)
     assert cn.dtype == dtype
     assert pytest.approx(cn) == ref
```

