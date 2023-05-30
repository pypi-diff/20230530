# Comparing `tmp/magentropy-0.1.3.tar.gz` & `tmp/magentropy-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magentropy-0.1.3.tar", last modified: Tue Jul 26 19:25:20 2022, max compression
+gzip compressed data, was "magentropy-0.1.4.tar", last modified: Tue May 30 03:21:55 2023, max compression
```

## Comparing `magentropy-0.1.3.tar` & `magentropy-0.1.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 soren      (503) staff       (20)        0 2022-07-26 19:25:20.182535 magentropy-0.1.3/
--rw-r--r--   0 soren      (503) staff       (20)     1067 2022-07-16 01:30:53.000000 magentropy-0.1.3/LICENSE
--rw-r--r--   0 soren      (503) staff       (20)      118 2022-07-22 18:33:35.000000 magentropy-0.1.3/MANIFEST.in
--rw-r--r--   0 soren      (503) staff       (20)     3788 2022-07-26 19:25:20.180897 magentropy-0.1.3/PKG-INFO
--rw-r--r--   0 soren      (503) staff       (20)     1503 2022-07-25 17:24:27.000000 magentropy-0.1.3/README.md
--rw-r--r--   0 soren      (503) staff       (20)     1806 2022-07-25 18:29:06.000000 magentropy-0.1.3/pyproject.toml
--rw-r--r--   0 soren      (503) staff       (20)       38 2022-07-26 19:25:20.184291 magentropy-0.1.3/setup.cfg
--rw-r--r--   0 soren      (503) staff       (20)      134 2022-07-16 18:23:23.000000 magentropy-0.1.3/setup.py
-drwxr-xr-x   0 soren      (503) staff       (20)        0 2022-07-26 19:25:20.141053 magentropy-0.1.3/src/
-drwxr-xr-x   0 soren      (503) staff       (20)        0 2022-07-26 19:25:20.146638 magentropy-0.1.3/src/_meta/
--rw-r--r--   0 soren      (503) staff       (20)      292 2022-07-25 18:29:06.000000 magentropy-0.1.3/src/_meta/__init__.py
-drwxr-xr-x   0 soren      (503) staff       (20)        0 2022-07-26 19:25:20.168929 magentropy-0.1.3/src/magentropy/
--rw-r--r--   0 soren      (503) staff       (20)      294 2022-07-20 20:40:18.000000 magentropy-0.1.3/src/magentropy/__init__.py
--rw-r--r--   0 soren      (503) staff       (20)    10777 2022-07-25 17:24:27.000000 magentropy-0.1.3/src/magentropy/_calculations.py
--rw-r--r--   0 soren      (503) staff       (20)     3359 2022-07-13 17:16:42.000000 magentropy-0.1.3/src/magentropy/_classvars.py
--rw-r--r--   0 soren      (503) staff       (20)     7519 2022-07-26 18:40:27.000000 magentropy-0.1.3/src/magentropy/_grouping.py
--rw-r--r--   0 soren      (503) staff       (20)     3699 2022-07-20 20:43:25.000000 magentropy-0.1.3/src/magentropy/_pint_utils.py
--rw-r--r--   0 soren      (503) staff       (20)    21820 2022-07-20 20:40:35.000000 magentropy-0.1.3/src/magentropy/_plotting.py
--rw-r--r--   0 soren      (503) staff       (20)    17450 2022-07-25 21:57:18.000000 magentropy-0.1.3/src/magentropy/_smoothing.py
--rw-r--r--   0 soren      (503) staff       (20)     9973 2022-07-25 17:24:27.000000 magentropy-0.1.3/src/magentropy/_validation.py
--rw-r--r--   0 soren      (503) staff       (20)      427 2022-07-19 20:59:26.000000 magentropy-0.1.3/src/magentropy/errors.py
--rw-r--r--   0 soren      (503) staff       (20)    89954 2022-07-26 18:45:02.000000 magentropy-0.1.3/src/magentropy/magentro.py
--rw-r--r--   0 soren      (503) staff       (20)     2801 2022-07-21 04:31:04.000000 magentropy-0.1.3/src/magentropy/typedefs.py
-drwxr-xr-x   0 soren      (503) staff       (20)        0 2022-07-26 19:25:20.177786 magentropy-0.1.3/src/magentropy.egg-info/
--rw-r--r--   0 soren      (503) staff       (20)      387 2022-07-26 19:25:20.000000 magentropy-0.1.3/src/magentropy.egg-info/SOURCES.txt
+drwxr-xr-x   0 soren      (503) staff       (20)        0 2023-05-30 03:21:55.366032 magentropy-0.1.4/
+-rw-r--r--   0 soren      (503) staff       (20)     1067 2022-08-04 18:11:46.000000 magentropy-0.1.4/LICENSE
+-rw-r--r--   0 soren      (503) staff       (20)      118 2022-08-04 18:11:46.000000 magentropy-0.1.4/MANIFEST.in
+-rw-r--r--   0 soren      (503) staff       (20)     3788 2023-05-30 03:21:55.365503 magentropy-0.1.4/PKG-INFO
+-rw-r--r--   0 soren      (503) staff       (20)     1503 2022-08-04 18:11:46.000000 magentropy-0.1.4/README.md
+-rw-r--r--   0 soren      (503) staff       (20)     1806 2022-08-04 18:11:46.000000 magentropy-0.1.4/pyproject.toml
+-rw-r--r--   0 soren      (503) staff       (20)       38 2023-05-30 03:21:55.366208 magentropy-0.1.4/setup.cfg
+-rw-r--r--   0 soren      (503) staff       (20)      134 2022-08-04 18:11:46.000000 magentropy-0.1.4/setup.py
+drwxr-xr-x   0 soren      (503) staff       (20)        0 2023-05-30 03:21:55.210654 magentropy-0.1.4/src/
+drwxr-xr-x   0 soren      (503) staff       (20)        0 2023-05-30 03:21:55.219285 magentropy-0.1.4/src/_meta/
+-rw-r--r--   0 soren      (503) staff       (20)      292 2022-08-04 18:11:46.000000 magentropy-0.1.4/src/_meta/__init__.py
+drwxr-xr-x   0 soren      (503) staff       (20)        0 2023-05-30 03:21:55.353512 magentropy-0.1.4/src/magentropy/
+-rw-r--r--   0 soren      (503) staff       (20)      294 2022-08-04 18:11:46.000000 magentropy-0.1.4/src/magentropy/__init__.py
+-rw-r--r--   0 soren      (503) staff       (20)    10813 2023-05-30 02:29:08.000000 magentropy-0.1.4/src/magentropy/_calculations.py
+-rw-r--r--   0 soren      (503) staff       (20)     3395 2023-05-30 02:29:02.000000 magentropy-0.1.4/src/magentropy/_classvars.py
+-rw-r--r--   0 soren      (503) staff       (20)     7555 2023-05-30 02:28:57.000000 magentropy-0.1.4/src/magentropy/_grouping.py
+-rw-r--r--   0 soren      (503) staff       (20)     3735 2023-05-30 02:28:53.000000 magentropy-0.1.4/src/magentropy/_pint_utils.py
+-rw-r--r--   0 soren      (503) staff       (20)    21856 2023-05-30 02:28:46.000000 magentropy-0.1.4/src/magentropy/_plotting.py
+-rw-r--r--   0 soren      (503) staff       (20)    17486 2023-05-30 02:28:38.000000 magentropy-0.1.4/src/magentropy/_smoothing.py
+-rw-r--r--   0 soren      (503) staff       (20)    10009 2023-05-30 02:28:28.000000 magentropy-0.1.4/src/magentropy/_validation.py
+-rw-r--r--   0 soren      (503) staff       (20)      427 2022-08-04 18:11:46.000000 magentropy-0.1.4/src/magentropy/errors.py
+-rw-r--r--   0 soren      (503) staff       (20)    89954 2022-08-04 18:11:46.000000 magentropy-0.1.4/src/magentropy/magentro.py
+-rw-r--r--   0 soren      (503) staff       (20)     2776 2023-05-30 02:27:46.000000 magentropy-0.1.4/src/magentropy/typedefs.py
+drwxr-xr-x   0 soren      (503) staff       (20)        0 2023-05-30 03:21:55.364797 magentropy-0.1.4/src/magentropy.egg-info/
+-rw-r--r--   0 soren      (503) staff       (20)      387 2023-05-30 03:21:55.000000 magentropy-0.1.4/src/magentropy.egg-info/SOURCES.txt
```

### Comparing `magentropy-0.1.3/LICENSE` & `magentropy-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `magentropy-0.1.3/PKG-INFO` & `magentropy-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magentropy
-Version: 0.1.3
+Version: 0.1.4
 Summary: Perform magnetoentropic mapping of magnetic materials based on DC magnetization data.
 Author-email: Soren Bear <sbear@ucsb.edu>
 License: MIT License
         
         Copyright (c) 2022 Soren Bear
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `magentropy-0.1.3/README.md` & `magentropy-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `magentropy-0.1.3/pyproject.toml` & `magentropy-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ['setuptools>=61.2.0', 'wheel']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'magentropy'
-version = '0.1.3'
+version = '0.1.4'
 description = 'Perform magnetoentropic mapping of magnetic materials based on DC magnetization data.'
 readme = 'README.md'
 requires-python = '>=3.9'
 license = { file = 'LICENSE' }
 authors = [{ name = 'Soren Bear', email = 'sbear@ucsb.edu' }]
 keywords = [
     'magentropy',
```

### Comparing `magentropy-0.1.3/src/magentropy/_calculations.py` & `magentropy-0.1.4/src/magentropy/_calculations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 '''
 Contains functions used for simulation, smoothing, interpolation, differentiation, and integration.
 '''
 
+from __future__ import annotations
+
 from typing import Union
 
 import numpy as np
 from numpy.typing import ArrayLike, NDArray
 import pandas as pd
 from pint import Quantity
 from scipy.integrate import cumulative_trapezoid
```

### Comparing `magentropy-0.1.3/src/magentropy/_classvars.py` & `magentropy-0.1.4/src/magentropy/_classvars.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 '''Contains some class variables so as to not clutter magentro.py.'''
 
+from __future__ import annotations
+
 import numpy as np
 
 # Order is important! Treat all as ordered dicts.
 # The dict values are safe to change, but not the keys.
 
 RAW_DF_COLUMNS = {
     'T': 'T',
```

### Comparing `magentropy-0.1.3/src/magentropy/_grouping.py` & `magentropy-0.1.4/src/magentropy/_grouping.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 '''Contains functions to group data by field or temperature.'''
 
+from __future__ import annotations
+
 from typing import Union, Optional
 
 import numpy as np
 from numpy.typing import NDArray
 import pandas as pd
 from pandas.core.groupby.generic import DataFrameGroupBy
 from numba import njit
```

### Comparing `magentropy-0.1.3/src/magentropy/_pint_utils.py` & `magentropy-0.1.4/src/magentropy/_pint_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 '''Contains convenience functions for working with Pint.'''
 
+from __future__ import annotations
+
 from typing import Optional, Sequence
 
 import numpy as np
 from numpy.typing import NDArray
 import pandas as pd
 from pint import UnitRegistry, Quantity
```

### Comparing `magentropy-0.1.3/src/magentropy/_plotting.py` & `magentropy-0.1.4/src/magentropy/_plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 '''Contains functions used for plotting data.'''
 
+from __future__ import annotations
+
 from typing import Union, Optional, Sequence
 
 import numpy as np
 from numpy.typing import ArrayLike, NDArray
 import pandas as pd
 import pint_pandas
 from pandas.core.groupby.generic import DataFrameGroupBy
```

### Comparing `magentropy-0.1.3/src/magentropy/_smoothing.py` & `magentropy-0.1.4/src/magentropy/_smoothing.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,16 @@
 #SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
 #LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
 #DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
 #THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 #(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 #OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+from __future__ import annotations
+
 from typing import Union, Optional
 import logging
 
 import numpy as np
 from numpy.typing import NDArray
 from scipy import optimize
 from numba import njit, prange
```

### Comparing `magentropy-0.1.3/src/magentropy/_validation.py` & `magentropy-0.1.4/src/magentropy/_validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 '''Contains functions used for argument validation.'''
 
+from __future__ import annotations
+
 from typing import Union, Optional, Sequence, Any, get_args
 from copy import deepcopy
 
 import numpy as np
 from numpy.typing import ArrayLike, NDArray
 import pandas as pd
```

### Comparing `magentropy-0.1.3/src/magentropy/magentro.py` & `magentropy-0.1.4/src/magentropy/magentro.py`

 * *Files identical despite different names*

### Comparing `magentropy-0.1.3/src/magentropy/typedefs.py` & `magentropy-0.1.4/src/magentropy/typedefs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 '''Type definitions.'''
 
 from __future__ import annotations
 
 from typing import Any, Union, Optional, TypedDict, Literal
 from numpy.random import Generator, BitGenerator, SeedSequence
-from numpy.typing import ArrayLike, _ArrayLikeInt_co
+from numpy.typing import ArrayLike
 from pandas._typing import FilePath, ReadCsvBuffer
 
 __all__ = [
     'ReadCsvFile', 'RngSeed', 'GriddataMethod', 'Kwargs', 'MatchErrStr', 'ToMinimizeStr',
     'PlotType', 'DataProp', 'PlotDataVersion', 'MapDataVersion', 'GroupingProp',
     'ColumnDataDict', 'Presets', 'SetterPresets'
 ]
 
 ReadCsvFile = Union[FilePath, ReadCsvBuffer[bytes], ReadCsvBuffer[str]]
 
-RngSeed = Optional[Union[_ArrayLikeInt_co, SeedSequence, BitGenerator, Generator]]
+RngSeed = Optional[Union[ArrayLike, SeedSequence, BitGenerator, Generator]]
 
 GriddataMethod = Literal['linear', 'nearest', 'cubic']
 
 Kwargs = dict[str, Any]
 
 MatchErrStr = Literal['min', 'mean', 'max']
```

