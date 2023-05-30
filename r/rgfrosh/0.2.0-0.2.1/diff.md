# Comparing `tmp/rgfrosh-0.2.0.tar.gz` & `tmp/rgfrosh-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rgfrosh-0.2.0.tar", last modified: Wed Apr 26 16:28:32 2023, max compression
+gzip compressed data, was "rgfrosh-0.2.1.tar", last modified: Tue May 30 14:13:37 2023, max compression
```

## Comparing `rgfrosh-0.2.0.tar` & `rgfrosh-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:28:32.455610 rgfrosh-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-26 16:28:16.000000 rgfrosh-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-04-26 16:28:32.455610 rgfrosh-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-04-26 16:28:16.000000 rgfrosh-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-26 16:28:16.000000 rgfrosh-0.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:28:32.455610 rgfrosh-0.2.0/rgfrosh/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-26 16:28:16.000000 rgfrosh-0.2.0/rgfrosh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-26 16:28:16.000000 rgfrosh-0.2.0/rgfrosh/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-26 16:28:16.000000 rgfrosh-0.2.0/rgfrosh/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    25006 2023-04-26 16:28:16.000000 rgfrosh-0.2.0/rgfrosh/shock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-04-26 16:28:16.000000 rgfrosh-0.2.0/rgfrosh/thermo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:28:32.455610 rgfrosh-0.2.0/rgfrosh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-04-26 16:28:32.000000 rgfrosh-0.2.0/rgfrosh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-26 16:28:32.000000 rgfrosh-0.2.0/rgfrosh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:28:32.000000 rgfrosh-0.2.0/rgfrosh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-26 16:28:32.000000 rgfrosh-0.2.0/rgfrosh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-26 16:28:32.000000 rgfrosh-0.2.0/rgfrosh.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-26 16:28:32.455610 rgfrosh-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:28:32.455610 rgfrosh-0.2.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-04-26 16:28:16.000000 rgfrosh-0.2.0/test/test_frozen_shock.py
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-04-26 16:28:16.000000 rgfrosh-0.2.0/test/test_ideal_shock.py
+drwxrwxrwx   0        0        0        0 2023-05-30 14:13:37.166467 rgfrosh-0.2.1/
+-rw-rw-rw-   0        0        0     1086 2023-05-30 01:31:18.000000 rgfrosh-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     4084 2023-05-30 14:13:37.166467 rgfrosh-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3379 2023-05-30 01:31:18.000000 rgfrosh-0.2.1/README.md
+-rw-rw-rw-   0        0        0      110 2023-05-30 01:31:18.000000 rgfrosh-0.2.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-30 14:13:37.139892 rgfrosh-0.2.1/rgfrosh/
+-rw-rw-rw-   0        0        0      144 2023-05-30 01:31:18.000000 rgfrosh-0.2.1/rgfrosh/__init__.py
+-rw-rw-rw-   0        0        0       82 2023-05-30 01:31:18.000000 rgfrosh-0.2.1/rgfrosh/constants.py
+-rw-rw-rw-   0        0        0      121 2023-05-30 01:31:18.000000 rgfrosh-0.2.1/rgfrosh/errors.py
+-rw-rw-rw-   0        0        0    25755 2023-05-30 01:31:18.000000 rgfrosh-0.2.1/rgfrosh/shock.py
+-rw-rw-rw-   0        0        0     3294 2023-05-30 01:31:18.000000 rgfrosh-0.2.1/rgfrosh/thermo.py
+drwxrwxrwx   0        0        0        0 2023-05-30 14:13:37.155948 rgfrosh-0.2.1/rgfrosh.egg-info/
+-rw-rw-rw-   0        0        0     4084 2023-05-30 14:13:37.000000 rgfrosh-0.2.1/rgfrosh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      341 2023-05-30 14:13:37.000000 rgfrosh-0.2.1/rgfrosh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 14:13:37.000000 rgfrosh-0.2.1/rgfrosh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-05-30 14:13:37.000000 rgfrosh-0.2.1/rgfrosh.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-30 14:13:37.000000 rgfrosh-0.2.1/rgfrosh.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      879 2023-05-30 14:13:37.168461 rgfrosh-0.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-30 14:13:37.165471 rgfrosh-0.2.1/test/
+-rw-rw-rw-   0        0        0     6262 2023-05-30 01:31:18.000000 rgfrosh-0.2.1/test/test_frozen_shock.py
+-rw-rw-rw-   0        0        0     4623 2023-05-30 01:31:18.000000 rgfrosh-0.2.1/test/test_ideal_shock.py
```

### Comparing `rgfrosh-0.2.0/PKG-INFO` & `rgfrosh-0.2.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,96 +1,98 @@
-Metadata-Version: 2.1
-Name: rgfrosh
-Version: 0.2.0
-Summary: A frozen shock solver for ideal and real gas equations of state.
-Home-page: https://github.com/VasuLab/RGFROSH
-Author: Cory Kinney
-Author-email: corykinney@ucf.edu
-License: MIT
-Platform: any
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Python Real Gas FROzen SHock (RGFROSH)
-
-![CI](https://github.com/VasuLab/RGFROSH/actions/workflows/main.yml/badge.svg?event=push)
-[![codecov](https://codecov.io/gh/VasuLab/RGFROSH/branch/main/graph/badge.svg?token=00W4E78FDD)](https://codecov.io/gh/VasuLab/RGFROSH)
-[![pypi](https://img.shields.io/pypi/v/rgfrosh.svg)](https://pypi.python.org/pypi/rgfrosh)
-[![versions](https://img.shields.io/pypi/pyversions/rgfrosh.svg)](https://github.com/VasuLab/rgfrosh)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
-[![license](https://img.shields.io/github/license/VasuLab/rgfrosh.svg)](https://github.com/VasuLab/rgfrosh/blob/main/LICENSE)
-[![DOI](https://zenodo.org/badge/435992350.svg)](https://zenodo.org/badge/latestdoi/435992350)
-
-> This project is a solver for the frozen shock equations[^1] developed in Python at the
-> University of Central Florida. The original RGFROSH was developed in FORTRAN at Stanford 
-> University by D. F. Davidson and R. K. Hanson using real gas subroutines for 
-> CHEMKIN[^2][^3]. 
-
-Python RGFROSH (`rgfrosh`) is a package for calculating conditions behind incident and reflected shock in
-a shock tube for an arbitrary equation of state. 
-
-## Documentation
-
-The [documentation site](https://vasulab.github.io/RGFROSH) provides a detailed 
-[user guide](https://vasulab.github.io/RGFROSH/guide/getting-started) and 
-[reference](https://vasulab.github.io/RGFROSH/reference) for the package.
-
-## Installation
-
-Python RGFROSH can be installed using
-
-```
-pip install rgfrosh
-```
-
-which also installs required dependencies. Cantera or CoolProp are optional and must
-be installed separately if desired.
-
-## Contributing
-
-For any bugs or feature requests, create an issue on the 
-[issue tracker](https://github.com/VasuLab/RGFROSH/issues). 
-
-After cloning the repository, the development environment can be set up with
-
-```
-pip install -r requirements.txt
-```
-
-Before creating a pull request, be sure to lint
-
-```
-black .
-```
-
-and run the automated tests
-
-```
-pytest
-```
-
-These checks will be performed automatically for all pull requests along
-with test coverage comparisons.
-
-## Cite
-
-To cite Python RGFROSH click <kbd>Cite this repository</kbd>on the right side of the GitHub repository
-page to export the citation for the latest release of `rgfrosh`. It is also encouraged to cite the 
-original paper[^1] for the frozen shock equations that this work is a derived from.
-
-
-[^1]: Davidson, D.F. and Hanson, R.K. (1996), Real Gas Corrections in Shock Tube Studies 
-at High Pressures. Isr. J. Chem., 36: 321-326. https://doi.org/10.1002/ijch.199600044
-[^2]: P. Barry Butler, "Real Gas Equations of State for Chemkin" Sandia Report No. 
-SAND88-3188 (1988). https://doi.org/10.2172/6224858
-[^3]: R. G. Schmitt, P. B. Butler, N. B. French "Chemkin real gas: a Fortran package for 
-analaysis of thermodynamic properties and chemical kinetics in non-ideal systems," 
-U. of Iowa Report UIME PPB 93-006 (1994).
+Metadata-Version: 2.1
+Name: rgfrosh
+Version: 0.2.1
+Summary: A frozen shock solver for ideal and real gas equations of state.
+Home-page: https://github.com/VasuLab/RGFROSH
+Author: Cory Kinney
+Author-email: corykinney@ucf.edu
+License: MIT
+Platform: any
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Python Real Gas FROzen SHock (RGFROSH)
+
+![CI](https://github.com/VasuLab/RGFROSH/actions/workflows/main.yml/badge.svg?event=push)
+[![codecov](https://codecov.io/gh/VasuLab/RGFROSH/branch/main/graph/badge.svg?token=00W4E78FDD)](https://codecov.io/gh/VasuLab/RGFROSH)
+[![pypi](https://img.shields.io/pypi/v/rgfrosh.svg)](https://pypi.python.org/pypi/rgfrosh)
+[![versions](https://img.shields.io/pypi/pyversions/rgfrosh.svg)](https://github.com/VasuLab/rgfrosh)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+[![license](https://img.shields.io/github/license/VasuLab/rgfrosh.svg)](https://github.com/VasuLab/rgfrosh/blob/main/LICENSE)
+[![DOI](https://zenodo.org/badge/435992350.svg)](https://zenodo.org/badge/latestdoi/435992350)
+
+> This project is a solver for the frozen shock equations[^1] developed in Python at the
+> University of Central Florida. The original RGFROSH was developed in FORTRAN at Stanford 
+> University by D. F. Davidson and R. K. Hanson using real gas subroutines for 
+> CHEMKIN[^2][^3]. 
+
+Python RGFROSH (`rgfrosh`) is a package for calculating conditions behind incident and reflected shock in
+a shock tube. As its name suggests, `rgfrosh` was written primarily for solving the frozen shock equations for
+a real gas equation of state; however, the implementation also allows for the use of the ideal gas equation of state or 
+even custom equations of state. Additionally, an implementation of the ideal shock equations is also available for comparison. 
+
+## Documentation
+
+The [documentation site](https://vasulab.github.io/RGFROSH) provides a detailed 
+[user guide](https://vasulab.github.io/RGFROSH/guide/getting-started) and 
+[reference](https://vasulab.github.io/RGFROSH/reference) for the package.
+
+## Installation
+
+Python RGFROSH can be installed using
+
+```
+pip install rgfrosh
+```
+
+which also installs required dependencies. Cantera or CoolProp are optional and must
+be installed separately if desired.
+
+## Contributing
+
+For any bugs or feature requests, create an issue on the 
+[issue tracker](https://github.com/VasuLab/RGFROSH/issues). 
+
+After cloning the repository, the development environment can be set up with
+
+```
+pip install -r requirements.txt
+```
+
+Before creating a pull request, be sure to lint
+
+```
+black .
+```
+
+and run the automated tests
+
+```
+pytest
+```
+
+These checks will be performed automatically for all pull requests along
+with test coverage comparisons.
+
+## Cite
+
+To cite Python RGFROSH click <kbd>Cite this repository</kbd>on the right side of the GitHub repository
+page to export the citation for the latest release of `rgfrosh`. It is also encouraged to cite the 
+original paper[^1] for the frozen shock equations that this work is a derived from.
+
+
+[^1]: Davidson, D.F. and Hanson, R.K. (1996), Real Gas Corrections in Shock Tube Studies 
+at High Pressures. Isr. J. Chem., 36: 321-326. https://doi.org/10.1002/ijch.199600044
+[^2]: P. Barry Butler, "Real Gas Equations of State for Chemkin" Sandia Report No. 
+SAND88-3188 (1988). https://doi.org/10.2172/6224858
+[^3]: R. G. Schmitt, P. B. Butler, N. B. French "Chemkin real gas: a Fortran package for 
+analaysis of thermodynamic properties and chemical kinetics in non-ideal systems," 
+U. of Iowa Report UIME PPB 93-006 (1994).
```

### Comparing `rgfrosh-0.2.0/README.md` & `rgfrosh-0.2.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,76 +1,78 @@
-# Python Real Gas FROzen SHock (RGFROSH)
-
-![CI](https://github.com/VasuLab/RGFROSH/actions/workflows/main.yml/badge.svg?event=push)
-[![codecov](https://codecov.io/gh/VasuLab/RGFROSH/branch/main/graph/badge.svg?token=00W4E78FDD)](https://codecov.io/gh/VasuLab/RGFROSH)
-[![pypi](https://img.shields.io/pypi/v/rgfrosh.svg)](https://pypi.python.org/pypi/rgfrosh)
-[![versions](https://img.shields.io/pypi/pyversions/rgfrosh.svg)](https://github.com/VasuLab/rgfrosh)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
-[![license](https://img.shields.io/github/license/VasuLab/rgfrosh.svg)](https://github.com/VasuLab/rgfrosh/blob/main/LICENSE)
-[![DOI](https://zenodo.org/badge/435992350.svg)](https://zenodo.org/badge/latestdoi/435992350)
-
-> This project is a solver for the frozen shock equations[^1] developed in Python at the
-> University of Central Florida. The original RGFROSH was developed in FORTRAN at Stanford 
-> University by D. F. Davidson and R. K. Hanson using real gas subroutines for 
-> CHEMKIN[^2][^3]. 
-
-Python RGFROSH (`rgfrosh`) is a package for calculating conditions behind incident and reflected shock in
-a shock tube for an arbitrary equation of state. 
-
-## Documentation
-
-The [documentation site](https://vasulab.github.io/RGFROSH) provides a detailed 
-[user guide](https://vasulab.github.io/RGFROSH/guide/getting-started) and 
-[reference](https://vasulab.github.io/RGFROSH/reference) for the package.
-
-## Installation
-
-Python RGFROSH can be installed using
-
-```
-pip install rgfrosh
-```
-
-which also installs required dependencies. Cantera or CoolProp are optional and must
-be installed separately if desired.
-
-## Contributing
-
-For any bugs or feature requests, create an issue on the 
-[issue tracker](https://github.com/VasuLab/RGFROSH/issues). 
-
-After cloning the repository, the development environment can be set up with
-
-```
-pip install -r requirements.txt
-```
-
-Before creating a pull request, be sure to lint
-
-```
-black .
-```
-
-and run the automated tests
-
-```
-pytest
-```
-
-These checks will be performed automatically for all pull requests along
-with test coverage comparisons.
-
-## Cite
-
-To cite Python RGFROSH click <kbd>Cite this repository</kbd>on the right side of the GitHub repository
-page to export the citation for the latest release of `rgfrosh`. It is also encouraged to cite the 
-original paper[^1] for the frozen shock equations that this work is a derived from.
-
-
-[^1]: Davidson, D.F. and Hanson, R.K. (1996), Real Gas Corrections in Shock Tube Studies 
-at High Pressures. Isr. J. Chem., 36: 321-326. https://doi.org/10.1002/ijch.199600044
-[^2]: P. Barry Butler, "Real Gas Equations of State for Chemkin" Sandia Report No. 
-SAND88-3188 (1988). https://doi.org/10.2172/6224858
-[^3]: R. G. Schmitt, P. B. Butler, N. B. French "Chemkin real gas: a Fortran package for 
-analaysis of thermodynamic properties and chemical kinetics in non-ideal systems," 
-U. of Iowa Report UIME PPB 93-006 (1994).
+# Python Real Gas FROzen SHock (RGFROSH)
+
+![CI](https://github.com/VasuLab/RGFROSH/actions/workflows/main.yml/badge.svg?event=push)
+[![codecov](https://codecov.io/gh/VasuLab/RGFROSH/branch/main/graph/badge.svg?token=00W4E78FDD)](https://codecov.io/gh/VasuLab/RGFROSH)
+[![pypi](https://img.shields.io/pypi/v/rgfrosh.svg)](https://pypi.python.org/pypi/rgfrosh)
+[![versions](https://img.shields.io/pypi/pyversions/rgfrosh.svg)](https://github.com/VasuLab/rgfrosh)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+[![license](https://img.shields.io/github/license/VasuLab/rgfrosh.svg)](https://github.com/VasuLab/rgfrosh/blob/main/LICENSE)
+[![DOI](https://zenodo.org/badge/435992350.svg)](https://zenodo.org/badge/latestdoi/435992350)
+
+> This project is a solver for the frozen shock equations[^1] developed in Python at the
+> University of Central Florida. The original RGFROSH was developed in FORTRAN at Stanford 
+> University by D. F. Davidson and R. K. Hanson using real gas subroutines for 
+> CHEMKIN[^2][^3]. 
+
+Python RGFROSH (`rgfrosh`) is a package for calculating conditions behind incident and reflected shock in
+a shock tube. As its name suggests, `rgfrosh` was written primarily for solving the frozen shock equations for
+a real gas equation of state; however, the implementation also allows for the use of the ideal gas equation of state or 
+even custom equations of state. Additionally, an implementation of the ideal shock equations is also available for comparison. 
+
+## Documentation
+
+The [documentation site](https://vasulab.github.io/RGFROSH) provides a detailed 
+[user guide](https://vasulab.github.io/RGFROSH/guide/getting-started) and 
+[reference](https://vasulab.github.io/RGFROSH/reference) for the package.
+
+## Installation
+
+Python RGFROSH can be installed using
+
+```
+pip install rgfrosh
+```
+
+which also installs required dependencies. Cantera or CoolProp are optional and must
+be installed separately if desired.
+
+## Contributing
+
+For any bugs or feature requests, create an issue on the 
+[issue tracker](https://github.com/VasuLab/RGFROSH/issues). 
+
+After cloning the repository, the development environment can be set up with
+
+```
+pip install -r requirements.txt
+```
+
+Before creating a pull request, be sure to lint
+
+```
+black .
+```
+
+and run the automated tests
+
+```
+pytest
+```
+
+These checks will be performed automatically for all pull requests along
+with test coverage comparisons.
+
+## Cite
+
+To cite Python RGFROSH click <kbd>Cite this repository</kbd>on the right side of the GitHub repository
+page to export the citation for the latest release of `rgfrosh`. It is also encouraged to cite the 
+original paper[^1] for the frozen shock equations that this work is a derived from.
+
+
+[^1]: Davidson, D.F. and Hanson, R.K. (1996), Real Gas Corrections in Shock Tube Studies 
+at High Pressures. Isr. J. Chem., 36: 321-326. https://doi.org/10.1002/ijch.199600044
+[^2]: P. Barry Butler, "Real Gas Equations of State for Chemkin" Sandia Report No. 
+SAND88-3188 (1988). https://doi.org/10.2172/6224858
+[^3]: R. G. Schmitt, P. B. Butler, N. B. French "Chemkin real gas: a Fortran package for 
+analaysis of thermodynamic properties and chemical kinetics in non-ideal systems," 
+U. of Iowa Report UIME PPB 93-006 (1994).
```

### Comparing `rgfrosh-0.2.0/rgfrosh/shock.py` & `rgfrosh-0.2.1/rgfrosh/shock.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,749 +1,749 @@
-from .thermo import ThermoInterface
-from .constants import GAS_CONSTANT
-from .errors import ConvergenceError
-
-from attrs import frozen
-from typing import Tuple
-
-import numpy as np
-
-
-@frozen
-class Shock:
-    u1: float
-    """Incident shock velocity [m/s]."""
-    T1: float
-    """Initial temperature [K]."""
-    P1: float
-    """Initial pressure [Pa]."""
-    rho1: float
-    """Initial density [kg/m^3^]."""
-
-    u2: float
-    """Velocity behind the incident shock (shock-fixed) [m/s]."""
-    T2: float
-    """Temperature behind the incident shock [K]."""
-    P2: float
-    """Pressure behind the incident shock [Pa]."""
-    rho2: float
-    """Density behind the incident shock [kg/m^3^]."""
-
-    u5: float
-    """Reflected shock velocity [m/s]."""
-    T5: float
-    """Temperature behind the reflected shock [K]."""
-    P5: float
-    """Pressure behind the reflected shock [Pa]."""
-    rho5: float
-    """Density behind the reflected shock [kg/m^3^]."""
-
-    MW: float
-    """Mean molecular weight [kg/kmol]."""
-
-
-class IdealShock(Shock):
-    """
-    A class for calculating properties in various regions of an ideal reflected shock. Most of
-    the equations implemented were derived in Gaydon and Hurle[^1].
-
-    !!! New "New in `v0.2.0`"
-
-    [^1]: Gaydon, A. G. and I. R. Hurle (1963). The shock tube in high-temperature chemical
-    physics, Reinhold Publishing Corporation.
-    """
-
-    def __init__(
-        self,
-        gamma: float,
-        MW: float,
-        *,
-        M: float = None,
-        u1: float = None,
-        T1: float = 300,
-        P1: float = None,
-        T5: float = None,
-        P5: float = None,
-    ):
-        r"""
-        Solves the ideal shock equations for the following combination of parameters:
-
-        1. Incident shock Mach number ($M$), or incident shock velocity ($u_1$), and initial conditions ($T_1$, $P_1$)
-        2. Reflected shock conditions ($T_5$, $P_5$) and initial temperature ($T_1$)
-
-        given the mixture's specific heat ratio ($\gamma$) and mean molecular weight ($\overline{M}$).
-        Density is calculated using the ideal gas law:
-
-        $$
-        \rho = \frac{P}{RT}
-        $$
-
-        where $R$ is the specific gas constant:
-
-        $$
-        R = R_\text{universal}/\overline{M}
-        $$
-
-        The speed of sound ($a$) is calculated as:
-
-        $$
-        a = \sqrt{\gamma R T}
-        $$
-
-        Arguments:
-            gamma: Specific heat ratio.
-            MW: Molecular weight [g/mol].
-
-        Keyword arguments:
-            u1: Incident shock velocity [m/s].
-            M: Incident shock Mach number.
-            T1: Initial temperature [K].
-            P1: Initial pressure [Pa].
-            T5: Temperature behind the reflected shock [K].
-            P5: Pressure behind the reflected shock [Pa].
-
-        Raises:
-            ValueError: If the system is underconstrained/overconstrained.
-
-        """
-
-        R = GAS_CONSTANT / MW
-        a1 = (gamma * R * T1) ** 0.5
-
-        if (M and T1 and P1) or (u1 and T1 and P1):
-            if (M and u1) or T5 or P5:
-                raise ValueError("Overconstrained - too many arguments provided.")
-
-            if M:
-                u1 = M * a1
-            else:
-                M = u1 / a1
-
-            P5 = P1 * IdealShock.reflected_pressure_ratio(M, gamma)
-            T5 = T1 * IdealShock.reflected_temperature_ratio(M, gamma)
-
-        elif T5 and P5 and T1:
-            if P1 or M or u1:
-                raise ValueError("Overconstrained - too many arguments provided.")
-
-            M = IdealShock.incident_Mach_number(gamma, T5, T1)
-            u1 = M * a1
-            P1 = P5 / IdealShock.reflected_pressure_ratio(M, gamma)
-
-        else:
-            raise ValueError("Underconstrained - insufficient arguments provided.")
-
-        P2 = P1 * IdealShock.incident_pressure_ratio(M, gamma)
-        T2 = T1 * IdealShock.incident_temperature_ratio(M, gamma)
-
-        rho1 = P1 / (R * T1)
-        rho2 = P2 / (R * T2)
-        rho5 = P5 / (R * T5)
-
-        u2 = u1 / IdealShock.incident_density_ratio(M, gamma)
-        u5 = u1 * IdealShock.reflected_velocity_ratio(M, gamma)
-
-        super().__init__(u1, T1, P1, rho1, u2, T2, P2, rho2, u5, T5, P5, rho5, MW)
-
-    @classmethod
-    def from_thermo(cls, thermo: ThermoInterface, **kwargs):
-        r"""
-        Alternative constructor from a `ThermoInterface` object.
-
-        For an ideal gas, the specific heat at constant volume ($c_v$) is related to the specific heat
-        at constant pressure ($c_p$) by the gas constant ($R$):
-
-        $$
-        c_p = c_v + R
-        $$
-
-        therefore, the specific heat ratio ($\gamma$) is calculated from the available properties as:
-
-        $$
-        \gamma = \frac{c_p}{c_p - R}
-        $$
-
-        !!! Note
-            $c_p$ is evaluated at the current state of the `thermo` object; therefore, the
-            calculated $\gamma$ may differ from the nominal value.
-        """
-        gamma = thermo.cp_mass / (
-            thermo.cp_mass - GAS_CONSTANT / thermo.mean_molecular_weight
-        )
-        return cls(gamma, thermo.mean_molecular_weight, **kwargs)
-
-    @staticmethod
-    def incident_pressure_ratio(M: float, gamma: float) -> float:
-        r"""
-        Calculates the pressure ratio across the incident shock:
-
-        $$
-        \frac{P_2}{P_1} = \frac{2\gamma M^2-(\gamma-1)}{\gamma+1}
-        $$
-
-        Parameters:
-            M: Incident shock Mach number.
-            gamma: Specific heat ratio.
-        """
-        return (2 * gamma * M**2 - (gamma - 1)) / (gamma + 1)
-
-    @staticmethod
-    def incident_temperature_ratio(M: float, gamma: float) -> float:
-        r"""
-        Calculates the temperature ratio across the incident shock:
-
-        $$
-        \frac{T_2}{T_1} = \frac{
-            \left(\gamma M^2 - \frac{\gamma-1}{2}\right)
-            \left(\frac{\gamma-1}{2}M^2+1\right)
-        }{
-            \left(\frac{\gamma+1}{2}\right)^2 M^2
-        }
-        $$
-
-        Parameters:
-            M: Incident shock Mach number.
-            gamma: Specific heat ratio.
-        """
-        return (
-            (gamma * M**2 - (gamma - 1) / 2)
-            * ((gamma - 1) / 2 * M**2 + 1)
-            / ((gamma + 1) / 2 * M) ** 2
-        )
-
-    @staticmethod
-    def incident_density_ratio(M: float, gamma: float) -> float:
-        r"""
-        Calculates the density ratio across the incident shock:
-
-        $$
-        \frac{\rho_2}{\rho_1} = \frac {(\gamma+1)M^2} {(\gamma-1)M^2+2}
-        $$
-
-        which is also the velocity ratio across the incident shock:
-
-        $$
-        \frac{u_1}{u_2} = \frac{\rho_2}{\rho_1}
-        $$
-
-        Parameters:
-            M: Incident shock Mach number.
-            gamma: Specific heat ratio.
-        """
-        return (gamma + 1) * M**2 / ((gamma - 1) * M**2 + 2)
-
-    @staticmethod
-    def reflected_pressure_ratio(M: float, gamma: float) -> float:
-        r"""
-        Calculates the ratio of the reflected shock pressure to the initial pressure:
-
-        $$
-        \frac{P_5}{P_1} = \left[\frac{2\gamma M^2-(\gamma-1)}{\gamma+1}\right]
-        \left[\frac{(3\gamma-1)M^2-2(\gamma-1)}{(\gamma-1)M^2+2}\right]
-        $$
-
-        Parameters:
-            M: Incident shock Mach number.
-            gamma: Specific heat ratio.
-        """
-        return (
-            (2 * gamma * M**2 - (gamma - 1))
-            / (gamma + 1)
-            * ((3 * gamma - 1) * M**2 - 2 * (gamma - 1))
-            / ((gamma - 1) * M**2 + 2)
-        )
-
-    @staticmethod
-    def reflected_temperature_ratio(M: float, gamma: float) -> float:
-        r"""
-        Calculates the ratio of the reflected shock temperature to the initial temperature:
-
-        $$
-        \frac{T_5}{T_1} = \frac{\left[2(\gamma-1)M^2+(3-\gamma)\right]
-        \left[(3\gamma-1)M^2-2(\gamma-1)\right]}
-        {(\gamma+1)^2M^2}
-        $$
-
-        Parameters:
-            M: Incident shock Mach number.
-            gamma: Specific heat ratio.
-        """
-        return (
-            (2 * (gamma - 1) * M**2 + 3 - gamma)
-            * ((3 * gamma - 1) * M**2 - 2 * (gamma - 1))
-            / ((gamma + 1) * M) ** 2
-        )
-
-    @staticmethod
-    def reflected_velocity_ratio(M: float, gamma: float) -> float:
-        r"""
-        Calculates the ratio of the reflected shock velocity to the incident shock velocity:
-
-        $$
-        \frac{V_R}{V_S} = \frac{2+\frac{2}{\gamma-1}\frac{P_1}{P_2}}
-        {\frac{\gamma+1}{\gamma-1}-\frac{P_1}{P_2}}
-        $$
-
-        Parameters:
-            M: Incident shock Mach number.
-            gamma: Specific heat ratio.
-        """
-        P12 = 1 / IdealShock.incident_pressure_ratio(M, gamma)
-        return (2 + 2 * P12 / (gamma - 1)) / ((gamma + 1) / (gamma - 1) - P12)
-
-    @staticmethod
-    def incident_Mach_number(gamma: float, T5: float, T1: float = 1):
-        r"""
-        Calculates the incident shock Mach number from the ratio of the reflected shock
-        temperature to the initial temperature. Expanding the equation for the reflected temperature
-        ratio yields an equation of the form:
-
-        $$
-        aM^4 + bM^2 + c = 0
-        $$
-
-        where
-
-        $$
-        a = 2(3\gamma-1)(\gamma-1)
-        $$
-
-        $$
-        b = (3\gamma-1)(3-\gamma) - 4(\gamma-1)^2 - \frac{T_5}{T_1}(\gamma+1)^2
-        $$
-
-        $$
-        c = -2(3-\gamma)(\gamma-1)
-        $$
-
-        Solving the above equation for $M^2$ using the quadratic formula, then taking the square
-        root of the non-negative solution, yields the incident shock Mach number for the given
-        temperature ratio:
-
-        $$
-        M = \sqrt{\frac{-b + \sqrt{b^2-4ac}}{2a}}
-        $$
-
-        Parameters:
-            gamma: Specific heat ratio.
-            T5: Reflected shock temperature [K].
-            T1: Initial temperature [K].
-
-        !!! Note
-            If `T1` is not specified, it is assumed that the temperature ratio ${T_5}/{T_1}$ is given as `T5`.
-
-        """
-        a = 2 * (gamma - 1) * (3 * gamma - 1)
-        b = (
-            (3 * gamma - 1) * (3 - gamma)
-            - 4 * (gamma - 1) ** 2
-            - (gamma + 1) ** 2 * T5 / T1
-        )
-        c = -2 * (gamma - 1) * (3 - gamma)
-
-        return ((-b + (b**2 - 4 * a * c) ** 0.5) / (2 * a)) ** 0.5
-
-
-class FrozenShock(Shock):
-    """
-    A class for calculating properties in various regions of a reflected shock given
-    the [`ThermoInterface`](../../thermo/#rgfrosh.thermo.ThermoInterface) for a mixture. The
-    [incident](rgfrosh.shock.FrozenShock.solve_incident) and
-    [reflected](rgfrosh.shock.FrozenShock.solve_reflected) solver equations are from Davidson and
-    Hanson[^1]. The equations for the
-    [initial conditions solver](rgfrosh.shock.FrozenShock.solve_initial) were derived in the appendix
-    of the cited dissertation[^2].
-
-    [^1]: Davidson, D. F. and R. K. Hanson (1996). "Real Gas Corrections in Shock Tube Studies at
-    High Pressures." Israel Journal of Chemistry 36(3): 321-326.
-    [^2]: Kinney, Cory, "Extreme-Pressure Ignition Studies of Methane and Natural Gas with CO2 with
-    Applications in Rockets and Gas Turbines" (2022). Electronic Theses and Dissertations, 2020-. 1033.
-    [https://stars.library.ucf.edu/etd2020/1033](https://stars.library.ucf.edu/etd2020/1033)
-    """
-
-    max_iter: int = 1000
-    """Maximum number of iterations for the solver."""
-
-    rtol: float = 1e-6
-    """Relative tolerance for the solver convergence criteria."""
-
-    def __init__(
-        self,
-        thermo: ThermoInterface,
-        *,
-        u1: float = None,
-        T1: float = 300,
-        P1: float = None,
-        T5: float = None,
-        P5: float = None,
-    ):
-        """
-        Solves the frozen shock equations for the following combination of parameters:
-
-        1. Incident shock velocity ($u_1$) and initial conditions ($T_1$, $P_1$)
-        2. Reflected shock conditions ($T_5$, $P_5$) and initial temperature ($T_1$)
-
-        Arguments:
-            thermo: Thermodynamic interface.
-
-        Keyword arguments:
-            u1: Incident shock velocity [m/s].
-            T1: Initial temperature [K].
-            P1: Initial pressure [Pa].
-            T5: Temperature behind the reflected shock [K].
-            P5: Pressure behind the reflected shock [Pa].
-
-        Raises:
-            ValueError: If the system is underconstrained/overconstrained.
-        """
-
-        MW = thermo.mean_molecular_weight
-
-        if u1 and T1 and P1:
-            if T5 or P5:
-                raise ValueError("Overconstrained - too many arguments provided.")
-
-            thermo.TP = T1, P1
-            rho1 = thermo.density_mass
-
-            u2, T2, P2, rho2 = FrozenShock.solve_incident(thermo, u1, T1, P1)
-            u5, T5, P5, rho5 = FrozenShock.solve_reflected(thermo, u1, P1, u2, T2, P2)
-
-        elif T5 and P5 and T1:
-            if P1 or u1:
-                raise ValueError("Overconstrained - too many arguments provided.")
-
-            u1, P1, u2, T2, P2, u5 = FrozenShock.solve_initial(thermo, T5, P5, T1)
-
-            thermo.TP = T1, P1
-            rho1 = thermo.density_mass
-            thermo.TP = T2, P2
-            rho2 = thermo.density_mass
-            thermo.TP = T5, P5
-            rho5 = thermo.density_mass
-
-        else:
-            raise ValueError("Underconstrained - insufficient arguments provided.")
-
-        super().__init__(u1, T1, P1, rho1, u2, T2, P2, rho2, u5, T5, P5, rho5, MW)
-
-    @property
-    def Z(self):
-        """
-        Compressibility factor ($Z$) at the reflected shock conditions.
-
-        !!! New "New in `v0.2.0`"
-        """
-        return self.P5 / (self.rho5 * GAS_CONSTANT / self.MW * self.T5)
-
-    @staticmethod
-    def solve_incident(
-        thermo: ThermoInterface,
-        u1: float,
-        T1: float,
-        P1: float,
-    ) -> Tuple[float, float, float, float]:
-        """
-        Solves for the conditions behind the incident shock.
-
-        Parameters:
-            thermo: Thermodynamic interface.
-            u1: Incident shock velocity [m/s].
-            T1: Initial temperature [K].
-            P1: Initial pressure [Pa].
-
-        Returns:
-            u2: Velocity behind the incident shock (shock-fixed) [m/s].
-            T2: Temperature behind the incident shock [K].
-            P2: Pressure behind the incident shock [Pa].
-            rho2: Density behind the incident shock [kg/m^3^].
-
-        Exceptions:
-            ConvergenceError: If the relative change in `T5` and `P5` is not below the
-                [`rtol`][rgfrosh.shock.FrozenShock.rtol] within
-                [`max_iter`][rgfrosh.shock.FrozenShock.max_iter] iterations.
-
-        """
-
-        thermo.TP = T1, P1
-        h1 = thermo.enthalpy_mass
-        nu1 = 1 / thermo.density_mass
-        cp1 = thermo.cp_mass
-
-        R = GAS_CONSTANT / thermo.mean_molecular_weight
-        gamma1 = cp1 / (cp1 - R)
-
-        # Calculate an initial guess of P2 and T2 with the ideal gas assumption
-        M1 = u1 / (gamma1 * R * T1) ** 0.5
-        T2 = T1 * (
-            (gamma1 * M1**2 - (gamma1 - 1) / 2)
-            * ((gamma1 - 1) / 2 * M1**2 + 1)
-            / ((gamma1 + 1) / 2 * M1) ** 2
-        )
-        P2 = P1 * (2 * gamma1 * M1**2 - (gamma1 - 1)) / (gamma1 + 1)
-
-        for i in range(FrozenShock.max_iter):
-            # Calculate thermodynamic properties at T2, P2 guess
-            thermo.TP = T2, P2
-            h2 = thermo.enthalpy_mass
-            nu2 = 1 / thermo.density_mass
-            cp2 = thermo.cp_mass
-            beta2 = thermo.thermal_expansion_coeff
-            kappa2 = thermo.isothermal_compressibility
-
-            f1 = (P2 / P1 - 1) + (u1**2 / (P1 * nu1)) * (nu2 / nu1 - 1)
-            f2 = ((h2 - h1) / (1 / 2 * u1**2)) + (nu2**2 / nu1**2 - 1)
-
-            df1_dT2 = u1**2 * nu2 * beta2 / (P1 * nu1**2)
-            df1_dP2 = 1 / P1 - u1**2 * nu2 * kappa2 / (P1 * nu1**2)
-
-            df2_dT2 = 2 * cp2 / u1**2 + 2 * (nu2 / nu1) ** 2 * beta2
-            df2_dP2 = (
-                2 * nu2 * (1 - T2 * beta2) / u1**2 - 2 * nu2**2 * kappa2 / nu1**2
-            )
-
-            deltaT2, deltaP2 = np.matmul(
-                np.linalg.inv(np.array([[df1_dT2, df1_dP2], [df2_dT2, df2_dP2]])),
-                np.array([f1, f2]),
-            )
-
-            converged = (
-                abs(deltaT2) <= T2 * FrozenShock.rtol
-                and abs(deltaP2) <= P2 * FrozenShock.rtol
-            )
-
-            T2 -= deltaT2
-            P2 -= deltaP2
-
-            if converged:
-                thermo.TP = T2, P2
-                nu2 = 1 / thermo.density_mass
-                u2 = u1 * nu2 / nu1
-                return u2, T2, P2, thermo.density_mass
-
-        raise ConvergenceError
-
-    @staticmethod
-    def solve_reflected(
-        thermo: ThermoInterface,
-        u1: float,
-        P1: float,
-        u2: float,
-        T2: float,
-        P2: float,
-    ) -> Tuple[float, float, float, float]:
-        """
-        Solves for the conditions behind the reflected shock.
-
-        Parameters:
-            thermo: Thermodynamic interface.
-            u1: Incident shock velocity [m/s].
-            P1: Initial pressure [Pa].
-            u2: Velocity behind the incident shock (shock-fixed) [m/s].
-            T2: Temperature behind the incident shock [K].
-            P2: Pressure behind the incident shock [Pa].
-
-        Returns:
-            u5: Reflected shock velocity [m/s].
-            T5: Temperature behind the reflected shock [K].
-            P5: Pressure behind the reflected shock [Pa].
-            rho5: Density behind the reflected shock [kg/m^3^].
-
-        Exceptions:
-            ConvergenceError: If the relative change in `T5` and `P5` is not below the
-                [`rtol`][rgfrosh.shock.FrozenShock.rtol] within
-                [`max_iter`][rgfrosh.shock.FrozenShock.max_iter] iterations.
-
-        """
-
-        thermo.TP = T2, P2
-        h2 = thermo.enthalpy_mass
-        nu2 = 1 / thermo.density_mass
-
-        # Calculate an initial guess of P5 and T5 with the ideal gas assumption
-        cp2 = thermo.cp_mass
-        R = GAS_CONSTANT / thermo.mean_molecular_weight
-        gamma2 = cp2 / (cp2 - R)
-
-        eta2 = (gamma2 + 1) / (gamma2 - 1)
-        P5 = P2 * (eta2 + 2 - P1 / P2) / (1 + eta2 * P1 / P2)
-        T5 = T2 * P5 / P2 * (eta2 + P5 / P2) / (1 + eta2 * P5 / P2)
-
-        for i in range(FrozenShock.max_iter):
-            thermo.TP = T5, P5
-
-            h5 = thermo.enthalpy_mass
-            nu5 = 1 / thermo.density_mass
-            cp5 = thermo.cp_mass
-            beta5 = thermo.thermal_expansion_coeff
-            kappa5 = thermo.isothermal_compressibility
-
-            f3 = (P5 / P2 - 1) + (u1 - u2) ** 2 / P2 / (nu5 - nu2)
-            f4 = 2 * (h5 - h2) / (u1 - u2) ** 2 + (nu5 + nu2) / (nu5 - nu2)
-
-            df3_dT5 = -nu5 * beta5 * (u1 - u2) ** 2 / (P2 * (nu5 - nu2) ** 2)
-            df3_dP5 = 1 / P2 + nu5 * kappa5 * (u1 - u2) ** 2 / (P2 * (nu5 - nu2) ** 2)
-
-            df4_dT5 = (
-                2 * cp5 / (u1 - u2) ** 2 - 2 * nu2 * nu5 * beta5 / (nu5 - nu2) ** 2
-            )
-            df4_dP5 = (
-                2 * nu5 * (1 - T5 * beta5) / (u1 - u2) ** 2
-                + 2 * nu2 * nu5 * kappa5 / (nu5 - nu2) ** 2
-            )
-
-            deltaT5, deltaP5 = np.matmul(
-                np.linalg.inv(np.array([[df3_dT5, df3_dP5], [df4_dT5, df4_dP5]])),
-                np.array([f3, f4]),
-            )
-
-            converged = (
-                abs(deltaT5) <= T5 * FrozenShock.rtol
-                and abs(deltaP5) <= P5 * FrozenShock.rtol
-            )
-
-            T5 -= deltaT5
-            P5 -= deltaP5
-
-            if converged:
-                thermo.TP = T5, P5
-                nu5 = 1 / thermo.density_mass
-                u5 = (u1 - u2) / (nu2 / nu5 - 1)
-                return u5, T5, P5, thermo.density_mass
-
-        raise ConvergenceError
-
-    @staticmethod
-    def solve_initial(thermo: ThermoInterface, T5: float, P5: float, T1: float = 300):
-        """
-        Solves for the initial pressure and incident shock velocity given the target
-        post-reflected-shock conditions.
-
-        Parameters:
-            thermo: Thermodynamic interface.
-            T5: Temperature behind the reflected shock [K].
-            P5: Pressure behind the reflected shock [Pa].
-            T1: Initial temperature [K].
-
-        Exceptions:
-            ConvergenceError: If the relative change in `u1`, `P1`, `T2`, and `P2`
-                is not below the [`rtol`][rgfrosh.shock.FrozenShock.rtol]
-                within [`max_iter`][rgfrosh.shock.FrozenShock.max_iter] iterations.
-
-        """
-
-        thermo.TP = T5, P5
-        h5 = thermo.enthalpy_mass
-        nu5 = 1 / thermo.density_mass
-
-        thermo.TP = T1, 101325
-        cp1 = thermo.cp_mass
-        R = GAS_CONSTANT / thermo.mean_molecular_weight
-        gamma1 = cp1 / (cp1 - R)
-        a1 = (gamma1 * GAS_CONSTANT / thermo.mean_molecular_weight * T1) ** 0.5
-
-        MS = IdealShock.incident_Mach_number(gamma1, T5, T1)
-        P1 = P5 / IdealShock.reflected_pressure_ratio(MS, gamma1)
-        P2 = P1 * IdealShock.incident_pressure_ratio(MS, gamma1)
-        T2 = T1 * IdealShock.incident_temperature_ratio(MS, gamma1)
-
-        u1 = MS * a1
-
-        for i in range(FrozenShock.max_iter):
-            thermo.TP = T1, P1
-            h1 = thermo.enthalpy_mass
-            nu1 = 1 / thermo.density_mass
-            beta1 = thermo.thermal_expansion_coeff
-            kappa1 = thermo.isothermal_compressibility
-
-            thermo.TP = T2, P2
-            h2 = thermo.enthalpy_mass
-            nu2 = 1 / thermo.density_mass
-            cp2 = thermo.cp_mass
-            beta2 = thermo.thermal_expansion_coeff
-            kappa2 = thermo.isothermal_compressibility
-
-            f1 = P2 / P1 - 1 + u1**2 / (P1 * nu1) * (nu2 / nu1 - 1)
-            f2 = 2 * (h2 - h1) / u1**2 + (nu2 / nu1) ** 2 - 1
-            f3 = (P5 / P2 - 1) + (u1 * (1 - nu2 / nu1)) ** 2 / P2 / (nu5 - nu2)
-            f4 = 2 * (h5 - h2) / (u1 * (1 - nu2 / nu1)) ** 2 + (nu5 + nu2) / (nu5 - nu2)
-
-            df1_du1 = 2 * u1 / (P1 * nu1**2) * (nu2 - nu1)
-            df1_dP1 = -P2 / P1**2 + u1**2 / (P1**2 * nu1**2) * (
-                P1 * kappa1 * (2 * nu2 - nu1) - (nu2 - nu1)
-            )
-            df1_dT2 = u1**2 * nu2 * beta2 / (P1 * nu1**2)
-            df1_dP2 = 1 / P1 - u1**2 * nu2 * kappa2 / (P1 * nu1**2)
-
-            df2_du1 = -4 * (h2 - h1) / u1**3
-            df2_dP1 = (
-                2 * nu2**2 * kappa1 / nu1**2 - 2 * nu1 * (1 - T1 * beta1) / u1**2
-            )
-            df2_dT2 = 2 * cp2 / u1**2 + 2 * (nu2 / nu1) ** 2 * beta2
-            df2_dP2 = (
-                2 * nu2 * (1 - T2 * beta2) / u1**2 - 2 * nu2**2 * kappa2 / nu1**2
-            )
-
-            df3_du1 = 2 * u1 * (1 - nu2 / nu1) ** 2 / (P2 * (nu5 - nu2))
-            df3_dP2 = -P5 / P2**2 - (
-                u1**2 / (nu1**2 * P2) * (nu1 - nu2) / (nu5 - nu2)
-            ) * (nu2 * kappa2 * (nu1 + nu2 - 2 * nu5) / (nu5 - nu2) + (nu1 - nu2) / P2)
-
-            df3_dT2 = (
-                (u1**2 * nu2 * beta2)
-                / (P2 * nu1**2)
-                * (nu1 - nu2)
-                / (nu5 - nu2) ** 2
-                * (nu1 + nu2 - 2 * nu5)
-            )
-            df4_dT2 = (2 * nu1**2 / u1**2) * (
-                2 * nu2 * beta2 * (h5 - h2) - cp2 * (nu1 - nu2)
-            ) / (nu1 - nu2) ** 3 + 2 * nu2 * nu5 * beta2 / (nu5 - nu2) ** 2
-            df4_dP2 = (-2 * nu1**2 * nu2) / u1**2 * (
-                2 * kappa2 * (h5 - h2) + (nu1 - nu2) * (1 - T2 * beta2)
-            ) / (nu1 - nu2) ** 3 - 2 * nu2 * nu5 * kappa2 / (nu5 - nu2) ** 2
-            df3_dP1 = (
-                -2 * u1**2 * nu2 * kappa1 * (1 - nu2 / nu1) / (P2 * nu1 * (nu5 - nu2))
-            )
-            df4_du1 = -4 * (h5 - h2) / (u1**3 * (1 - nu2 / nu1) ** 2)
-            df4_dP1 = (
-                4 * nu2 * kappa1 * (h5 - h2) / (u1**2 * nu1) / (1 - nu2 / nu1) ** 3
-            )
-
-            delta_u1, delta_P1, delta_T2, delta_P2 = np.matmul(
-                np.linalg.inv(
-                    np.array(
-                        [
-                            [df1_du1, df1_dP1, df1_dT2, df1_dP2],
-                            [df2_du1, df2_dP1, df2_dT2, df2_dP2],
-                            [df3_du1, df3_dP1, df3_dT2, df3_dP2],
-                            [df4_du1, df4_dP1, df4_dT2, df4_dP2],
-                        ]
-                    )
-                ),
-                np.array([f1, f2, f3, f4]),
-            )
-
-            converged = (
-                abs(delta_u1) <= u1 * FrozenShock.rtol
-                and abs(delta_P1) <= P1 * FrozenShock.rtol
-                and abs(delta_T2) <= T2 * FrozenShock.rtol
-                and abs(delta_P2) <= P2 * FrozenShock.rtol
-            )
-
-            u1 -= delta_u1
-            P1 -= delta_P1
-            T2 -= delta_T2
-            P2 -= delta_P2
-
-            if converged:
-                thermo.TP = T1, P1
-                rho1 = thermo.density_mass
-                thermo.TP = T2, P2
-                rho2 = thermo.density_mass
-
-                u2 = u1 * rho1 / rho2
-                u5 = (u1 - u2) / (nu2 / nu5 - 1)
-
-                return u1, P1, u2, T2, P2, u5
-
-        raise ConvergenceError
+from .thermo import ThermoInterface
+from .constants import GAS_CONSTANT
+from .errors import ConvergenceError
+
+from attrs import frozen
+from typing import Tuple
+
+import numpy as np
+
+
+@frozen
+class Shock:
+    u1: float
+    """Incident shock velocity [m/s]."""
+    T1: float
+    """Initial temperature [K]."""
+    P1: float
+    """Initial pressure [Pa]."""
+    rho1: float
+    """Initial density [kg/m^3^]."""
+
+    u2: float
+    """Velocity behind the incident shock (shock-fixed) [m/s]."""
+    T2: float
+    """Temperature behind the incident shock [K]."""
+    P2: float
+    """Pressure behind the incident shock [Pa]."""
+    rho2: float
+    """Density behind the incident shock [kg/m^3^]."""
+
+    u5: float
+    """Reflected shock velocity [m/s]."""
+    T5: float
+    """Temperature behind the reflected shock [K]."""
+    P5: float
+    """Pressure behind the reflected shock [Pa]."""
+    rho5: float
+    """Density behind the reflected shock [kg/m^3^]."""
+
+    MW: float
+    """Mean molecular weight [kg/kmol]."""
+
+
+class IdealShock(Shock):
+    """
+    A class for calculating properties in various regions of an ideal reflected shock. Most of
+    the equations implemented were derived in Gaydon and Hurle[^1].
+
+    !!! New "New in `v0.2.0`"
+
+    [^1]: Gaydon, A. G. and I. R. Hurle (1963). The shock tube in high-temperature chemical
+    physics, Reinhold Publishing Corporation.
+    """
+
+    def __init__(
+        self,
+        gamma: float,
+        MW: float,
+        *,
+        M: float = None,
+        u1: float = None,
+        T1: float = 300,
+        P1: float = None,
+        T5: float = None,
+        P5: float = None,
+    ):
+        r"""
+        Solves the ideal shock equations for the following combination of parameters:
+
+        1. Incident shock Mach number ($M$), or incident shock velocity ($u_1$), and initial conditions ($T_1$, $P_1$)
+        2. Reflected shock conditions ($T_5$, $P_5$) and initial temperature ($T_1$)
+
+        given the mixture's specific heat ratio ($\gamma$) and mean molecular weight ($\overline{M}$).
+        Density is calculated using the ideal gas law:
+
+        $$
+        \rho = \frac{P}{RT}
+        $$
+
+        where $R$ is the specific gas constant:
+
+        $$
+        R = R_\text{universal}/\overline{M}
+        $$
+
+        The speed of sound ($a$) is calculated as:
+
+        $$
+        a = \sqrt{\gamma R T}
+        $$
+
+        Arguments:
+            gamma: Specific heat ratio.
+            MW: Molecular weight [g/mol].
+
+        Keyword arguments:
+            u1: Incident shock velocity [m/s].
+            M: Incident shock Mach number.
+            T1: Initial temperature [K].
+            P1: Initial pressure [Pa].
+            T5: Temperature behind the reflected shock [K].
+            P5: Pressure behind the reflected shock [Pa].
+
+        Raises:
+            ValueError: If the system is underconstrained/overconstrained.
+
+        """
+
+        R = GAS_CONSTANT / MW
+        a1 = (gamma * R * T1) ** 0.5
+
+        if (M and T1 and P1) or (u1 and T1 and P1):
+            if (M and u1) or T5 or P5:
+                raise ValueError("Overconstrained - too many arguments provided.")
+
+            if M:
+                u1 = M * a1
+            else:
+                M = u1 / a1
+
+            P5 = P1 * IdealShock.reflected_pressure_ratio(M, gamma)
+            T5 = T1 * IdealShock.reflected_temperature_ratio(M, gamma)
+
+        elif T5 and P5 and T1:
+            if P1 or M or u1:
+                raise ValueError("Overconstrained - too many arguments provided.")
+
+            M = IdealShock.incident_Mach_number(gamma, T5, T1)
+            u1 = M * a1
+            P1 = P5 / IdealShock.reflected_pressure_ratio(M, gamma)
+
+        else:
+            raise ValueError("Underconstrained - insufficient arguments provided.")
+
+        P2 = P1 * IdealShock.incident_pressure_ratio(M, gamma)
+        T2 = T1 * IdealShock.incident_temperature_ratio(M, gamma)
+
+        rho1 = P1 / (R * T1)
+        rho2 = P2 / (R * T2)
+        rho5 = P5 / (R * T5)
+
+        u2 = u1 / IdealShock.incident_density_ratio(M, gamma)
+        u5 = u1 * IdealShock.reflected_velocity_ratio(M, gamma)
+
+        super().__init__(u1, T1, P1, rho1, u2, T2, P2, rho2, u5, T5, P5, rho5, MW)
+
+    @classmethod
+    def from_thermo(cls, thermo: ThermoInterface, **kwargs):
+        r"""
+        Alternative constructor from a `ThermoInterface` object.
+
+        For an ideal gas, the specific heat at constant volume ($c_v$) is related to the specific heat
+        at constant pressure ($c_p$) by the gas constant ($R$):
+
+        $$
+        c_p = c_v + R
+        $$
+
+        therefore, the specific heat ratio ($\gamma$) is calculated from the available properties as:
+
+        $$
+        \gamma = \frac{c_p}{c_p - R}
+        $$
+
+        !!! Note
+            $c_p$ is evaluated at the current state of the `thermo` object; therefore, the
+            calculated $\gamma$ may differ from the nominal value.
+        """
+        gamma = thermo.cp_mass / (
+            thermo.cp_mass - GAS_CONSTANT / thermo.mean_molecular_weight
+        )
+        return cls(gamma, thermo.mean_molecular_weight, **kwargs)
+
+    @staticmethod
+    def incident_pressure_ratio(M: float, gamma: float) -> float:
+        r"""
+        Calculates the pressure ratio across the incident shock:
+
+        $$
+        \frac{P_2}{P_1} = \frac{2\gamma M^2-(\gamma-1)}{\gamma+1}
+        $$
+
+        Parameters:
+            M: Incident shock Mach number.
+            gamma: Specific heat ratio.
+        """
+        return (2 * gamma * M**2 - (gamma - 1)) / (gamma + 1)
+
+    @staticmethod
+    def incident_temperature_ratio(M: float, gamma: float) -> float:
+        r"""
+        Calculates the temperature ratio across the incident shock:
+
+        $$
+        \frac{T_2}{T_1} = \frac{
+            \left(\gamma M^2 - \frac{\gamma-1}{2}\right)
+            \left(\frac{\gamma-1}{2}M^2+1\right)
+        }{
+            \left(\frac{\gamma+1}{2}\right)^2 M^2
+        }
+        $$
+
+        Parameters:
+            M: Incident shock Mach number.
+            gamma: Specific heat ratio.
+        """
+        return (
+            (gamma * M**2 - (gamma - 1) / 2)
+            * ((gamma - 1) / 2 * M**2 + 1)
+            / ((gamma + 1) / 2 * M) ** 2
+        )
+
+    @staticmethod
+    def incident_density_ratio(M: float, gamma: float) -> float:
+        r"""
+        Calculates the density ratio across the incident shock:
+
+        $$
+        \frac{\rho_2}{\rho_1} = \frac {(\gamma+1)M^2} {(\gamma-1)M^2+2}
+        $$
+
+        which is also the velocity ratio across the incident shock:
+
+        $$
+        \frac{u_1}{u_2} = \frac{\rho_2}{\rho_1}
+        $$
+
+        Parameters:
+            M: Incident shock Mach number.
+            gamma: Specific heat ratio.
+        """
+        return (gamma + 1) * M**2 / ((gamma - 1) * M**2 + 2)
+
+    @staticmethod
+    def reflected_pressure_ratio(M: float, gamma: float) -> float:
+        r"""
+        Calculates the ratio of the reflected shock pressure to the initial pressure:
+
+        $$
+        \frac{P_5}{P_1} = \left[\frac{2\gamma M^2-(\gamma-1)}{\gamma+1}\right]
+        \left[\frac{(3\gamma-1)M^2-2(\gamma-1)}{(\gamma-1)M^2+2}\right]
+        $$
+
+        Parameters:
+            M: Incident shock Mach number.
+            gamma: Specific heat ratio.
+        """
+        return (
+            (2 * gamma * M**2 - (gamma - 1))
+            / (gamma + 1)
+            * ((3 * gamma - 1) * M**2 - 2 * (gamma - 1))
+            / ((gamma - 1) * M**2 + 2)
+        )
+
+    @staticmethod
+    def reflected_temperature_ratio(M: float, gamma: float) -> float:
+        r"""
+        Calculates the ratio of the reflected shock temperature to the initial temperature:
+
+        $$
+        \frac{T_5}{T_1} = \frac{\left[2(\gamma-1)M^2+(3-\gamma)\right]
+        \left[(3\gamma-1)M^2-2(\gamma-1)\right]}
+        {(\gamma+1)^2M^2}
+        $$
+
+        Parameters:
+            M: Incident shock Mach number.
+            gamma: Specific heat ratio.
+        """
+        return (
+            (2 * (gamma - 1) * M**2 + 3 - gamma)
+            * ((3 * gamma - 1) * M**2 - 2 * (gamma - 1))
+            / ((gamma + 1) * M) ** 2
+        )
+
+    @staticmethod
+    def reflected_velocity_ratio(M: float, gamma: float) -> float:
+        r"""
+        Calculates the ratio of the reflected shock velocity to the incident shock velocity:
+
+        $$
+        \frac{V_R}{V_S} = \frac{2+\frac{2}{\gamma-1}\frac{P_1}{P_2}}
+        {\frac{\gamma+1}{\gamma-1}-\frac{P_1}{P_2}}
+        $$
+
+        Parameters:
+            M: Incident shock Mach number.
+            gamma: Specific heat ratio.
+        """
+        P12 = 1 / IdealShock.incident_pressure_ratio(M, gamma)
+        return (2 + 2 * P12 / (gamma - 1)) / ((gamma + 1) / (gamma - 1) - P12)
+
+    @staticmethod
+    def incident_Mach_number(gamma: float, T5: float, T1: float = 1):
+        r"""
+        Calculates the incident shock Mach number from the ratio of the reflected shock
+        temperature to the initial temperature. Expanding the equation for the reflected temperature
+        ratio yields an equation of the form:
+
+        $$
+        aM^4 + bM^2 + c = 0
+        $$
+
+        where
+
+        $$
+        a = 2(3\gamma-1)(\gamma-1)
+        $$
+
+        $$
+        b = (3\gamma-1)(3-\gamma) - 4(\gamma-1)^2 - \frac{T_5}{T_1}(\gamma+1)^2
+        $$
+
+        $$
+        c = -2(3-\gamma)(\gamma-1)
+        $$
+
+        Solving the above equation for $M^2$ using the quadratic formula, then taking the square
+        root of the non-negative solution, yields the incident shock Mach number for the given
+        temperature ratio:
+
+        $$
+        M = \sqrt{\frac{-b + \sqrt{b^2-4ac}}{2a}}
+        $$
+
+        Parameters:
+            gamma: Specific heat ratio.
+            T5: Reflected shock temperature [K].
+            T1: Initial temperature [K].
+
+        !!! Note
+            If `T1` is not specified, it is assumed that the temperature ratio ${T_5}/{T_1}$ is given as `T5`.
+
+        """
+        a = 2 * (gamma - 1) * (3 * gamma - 1)
+        b = (
+            (3 * gamma - 1) * (3 - gamma)
+            - 4 * (gamma - 1) ** 2
+            - (gamma + 1) ** 2 * T5 / T1
+        )
+        c = -2 * (gamma - 1) * (3 - gamma)
+
+        return ((-b + (b**2 - 4 * a * c) ** 0.5) / (2 * a)) ** 0.5
+
+
+class FrozenShock(Shock):
+    """
+    A class for calculating properties in various regions of a reflected shock given
+    the [`ThermoInterface`](../../thermo/#rgfrosh.thermo.ThermoInterface) for a mixture. The
+    [incident](rgfrosh.shock.FrozenShock.solve_incident) and
+    [reflected](rgfrosh.shock.FrozenShock.solve_reflected) solver equations are from Davidson and
+    Hanson[^1]. The equations for the
+    [initial conditions solver](rgfrosh.shock.FrozenShock.solve_initial) were derived in the appendix
+    of the cited dissertation[^2].
+
+    [^1]: Davidson, D. F. and R. K. Hanson (1996). "Real Gas Corrections in Shock Tube Studies at
+    High Pressures." Israel Journal of Chemistry 36(3): 321-326.
+    [^2]: Kinney, Cory, "Extreme-Pressure Ignition Studies of Methane and Natural Gas with CO2 with
+    Applications in Rockets and Gas Turbines" (2022). Electronic Theses and Dissertations, 2020-. 1033.
+    [https://stars.library.ucf.edu/etd2020/1033](https://stars.library.ucf.edu/etd2020/1033)
+    """
+
+    max_iter: int = 1000
+    """Maximum number of iterations for the solver."""
+
+    rtol: float = 1e-6
+    """Relative tolerance for the solver convergence criteria."""
+
+    def __init__(
+        self,
+        thermo: ThermoInterface,
+        *,
+        u1: float = None,
+        T1: float = 300,
+        P1: float = None,
+        T5: float = None,
+        P5: float = None,
+    ):
+        """
+        Solves the frozen shock equations for the following combination of parameters:
+
+        1. Incident shock velocity ($u_1$) and initial conditions ($T_1$, $P_1$)
+        2. Reflected shock conditions ($T_5$, $P_5$) and initial temperature ($T_1$)
+
+        Arguments:
+            thermo: Thermodynamic interface.
+
+        Keyword arguments:
+            u1: Incident shock velocity [m/s].
+            T1: Initial temperature [K].
+            P1: Initial pressure [Pa].
+            T5: Temperature behind the reflected shock [K].
+            P5: Pressure behind the reflected shock [Pa].
+
+        Raises:
+            ValueError: If the system is underconstrained/overconstrained.
+        """
+
+        MW = thermo.mean_molecular_weight
+
+        if u1 and T1 and P1:
+            if T5 or P5:
+                raise ValueError("Overconstrained - too many arguments provided.")
+
+            thermo.TP = T1, P1
+            rho1 = thermo.density_mass
+
+            u2, T2, P2, rho2 = FrozenShock.solve_incident(thermo, u1, T1, P1)
+            u5, T5, P5, rho5 = FrozenShock.solve_reflected(thermo, u1, P1, u2, T2, P2)
+
+        elif T5 and P5 and T1:
+            if P1 or u1:
+                raise ValueError("Overconstrained - too many arguments provided.")
+
+            u1, P1, u2, T2, P2, u5 = FrozenShock.solve_initial(thermo, T5, P5, T1)
+
+            thermo.TP = T1, P1
+            rho1 = thermo.density_mass
+            thermo.TP = T2, P2
+            rho2 = thermo.density_mass
+            thermo.TP = T5, P5
+            rho5 = thermo.density_mass
+
+        else:
+            raise ValueError("Underconstrained - insufficient arguments provided.")
+
+        super().__init__(u1, T1, P1, rho1, u2, T2, P2, rho2, u5, T5, P5, rho5, MW)
+
+    @property
+    def Z(self):
+        """
+        Compressibility factor ($Z$) at the reflected shock conditions.
+
+        !!! New "New in `v0.2.0`"
+        """
+        return self.P5 / (self.rho5 * GAS_CONSTANT / self.MW * self.T5)
+
+    @staticmethod
+    def solve_incident(
+        thermo: ThermoInterface,
+        u1: float,
+        T1: float,
+        P1: float,
+    ) -> Tuple[float, float, float, float]:
+        """
+        Solves for the conditions behind the incident shock.
+
+        Parameters:
+            thermo: Thermodynamic interface.
+            u1: Incident shock velocity [m/s].
+            T1: Initial temperature [K].
+            P1: Initial pressure [Pa].
+
+        Returns:
+            u2: Velocity behind the incident shock (shock-fixed) [m/s].
+            T2: Temperature behind the incident shock [K].
+            P2: Pressure behind the incident shock [Pa].
+            rho2: Density behind the incident shock [kg/m^3^].
+
+        Exceptions:
+            ConvergenceError: If the relative change in `T5` and `P5` is not below the
+                [`rtol`][rgfrosh.shock.FrozenShock.rtol] within
+                [`max_iter`][rgfrosh.shock.FrozenShock.max_iter] iterations.
+
+        """
+
+        thermo.TP = T1, P1
+        h1 = thermo.enthalpy_mass
+        nu1 = 1 / thermo.density_mass
+        cp1 = thermo.cp_mass
+
+        R = GAS_CONSTANT / thermo.mean_molecular_weight
+        gamma1 = cp1 / (cp1 - R)
+
+        # Calculate an initial guess of P2 and T2 with the ideal gas assumption
+        M1 = u1 / (gamma1 * R * T1) ** 0.5
+        T2 = T1 * (
+            (gamma1 * M1**2 - (gamma1 - 1) / 2)
+            * ((gamma1 - 1) / 2 * M1**2 + 1)
+            / ((gamma1 + 1) / 2 * M1) ** 2
+        )
+        P2 = P1 * (2 * gamma1 * M1**2 - (gamma1 - 1)) / (gamma1 + 1)
+
+        for i in range(FrozenShock.max_iter):
+            # Calculate thermodynamic properties at T2, P2 guess
+            thermo.TP = T2, P2
+            h2 = thermo.enthalpy_mass
+            nu2 = 1 / thermo.density_mass
+            cp2 = thermo.cp_mass
+            beta2 = thermo.thermal_expansion_coeff
+            kappa2 = thermo.isothermal_compressibility
+
+            f1 = (P2 / P1 - 1) + (u1**2 / (P1 * nu1)) * (nu2 / nu1 - 1)
+            f2 = ((h2 - h1) / (1 / 2 * u1**2)) + (nu2**2 / nu1**2 - 1)
+
+            df1_dT2 = u1**2 * nu2 * beta2 / (P1 * nu1**2)
+            df1_dP2 = 1 / P1 - u1**2 * nu2 * kappa2 / (P1 * nu1**2)
+
+            df2_dT2 = 2 * cp2 / u1**2 + 2 * (nu2 / nu1) ** 2 * beta2
+            df2_dP2 = (
+                2 * nu2 * (1 - T2 * beta2) / u1**2 - 2 * nu2**2 * kappa2 / nu1**2
+            )
+
+            deltaT2, deltaP2 = np.matmul(
+                np.linalg.inv(np.array([[df1_dT2, df1_dP2], [df2_dT2, df2_dP2]])),
+                np.array([f1, f2]),
+            )
+
+            converged = (
+                abs(deltaT2) <= T2 * FrozenShock.rtol
+                and abs(deltaP2) <= P2 * FrozenShock.rtol
+            )
+
+            T2 -= deltaT2
+            P2 -= deltaP2
+
+            if converged:
+                thermo.TP = T2, P2
+                nu2 = 1 / thermo.density_mass
+                u2 = u1 * nu2 / nu1
+                return u2, T2, P2, thermo.density_mass
+
+        raise ConvergenceError
+
+    @staticmethod
+    def solve_reflected(
+        thermo: ThermoInterface,
+        u1: float,
+        P1: float,
+        u2: float,
+        T2: float,
+        P2: float,
+    ) -> Tuple[float, float, float, float]:
+        """
+        Solves for the conditions behind the reflected shock.
+
+        Parameters:
+            thermo: Thermodynamic interface.
+            u1: Incident shock velocity [m/s].
+            P1: Initial pressure [Pa].
+            u2: Velocity behind the incident shock (shock-fixed) [m/s].
+            T2: Temperature behind the incident shock [K].
+            P2: Pressure behind the incident shock [Pa].
+
+        Returns:
+            u5: Reflected shock velocity [m/s].
+            T5: Temperature behind the reflected shock [K].
+            P5: Pressure behind the reflected shock [Pa].
+            rho5: Density behind the reflected shock [kg/m^3^].
+
+        Exceptions:
+            ConvergenceError: If the relative change in `T5` and `P5` is not below the
+                [`rtol`][rgfrosh.shock.FrozenShock.rtol] within
+                [`max_iter`][rgfrosh.shock.FrozenShock.max_iter] iterations.
+
+        """
+
+        thermo.TP = T2, P2
+        h2 = thermo.enthalpy_mass
+        nu2 = 1 / thermo.density_mass
+
+        # Calculate an initial guess of P5 and T5 with the ideal gas assumption
+        cp2 = thermo.cp_mass
+        R = GAS_CONSTANT / thermo.mean_molecular_weight
+        gamma2 = cp2 / (cp2 - R)
+
+        eta2 = (gamma2 + 1) / (gamma2 - 1)
+        P5 = P2 * (eta2 + 2 - P1 / P2) / (1 + eta2 * P1 / P2)
+        T5 = T2 * P5 / P2 * (eta2 + P5 / P2) / (1 + eta2 * P5 / P2)
+
+        for i in range(FrozenShock.max_iter):
+            thermo.TP = T5, P5
+
+            h5 = thermo.enthalpy_mass
+            nu5 = 1 / thermo.density_mass
+            cp5 = thermo.cp_mass
+            beta5 = thermo.thermal_expansion_coeff
+            kappa5 = thermo.isothermal_compressibility
+
+            f3 = (P5 / P2 - 1) + (u1 - u2) ** 2 / P2 / (nu5 - nu2)
+            f4 = 2 * (h5 - h2) / (u1 - u2) ** 2 + (nu5 + nu2) / (nu5 - nu2)
+
+            df3_dT5 = -nu5 * beta5 * (u1 - u2) ** 2 / (P2 * (nu5 - nu2) ** 2)
+            df3_dP5 = 1 / P2 + nu5 * kappa5 * (u1 - u2) ** 2 / (P2 * (nu5 - nu2) ** 2)
+
+            df4_dT5 = (
+                2 * cp5 / (u1 - u2) ** 2 - 2 * nu2 * nu5 * beta5 / (nu5 - nu2) ** 2
+            )
+            df4_dP5 = (
+                2 * nu5 * (1 - T5 * beta5) / (u1 - u2) ** 2
+                + 2 * nu2 * nu5 * kappa5 / (nu5 - nu2) ** 2
+            )
+
+            deltaT5, deltaP5 = np.matmul(
+                np.linalg.inv(np.array([[df3_dT5, df3_dP5], [df4_dT5, df4_dP5]])),
+                np.array([f3, f4]),
+            )
+
+            converged = (
+                abs(deltaT5) <= T5 * FrozenShock.rtol
+                and abs(deltaP5) <= P5 * FrozenShock.rtol
+            )
+
+            T5 -= deltaT5
+            P5 -= deltaP5
+
+            if converged:
+                thermo.TP = T5, P5
+                nu5 = 1 / thermo.density_mass
+                u5 = (u1 - u2) / (nu2 / nu5 - 1)
+                return u5, T5, P5, thermo.density_mass
+
+        raise ConvergenceError
+
+    @staticmethod
+    def solve_initial(thermo: ThermoInterface, T5: float, P5: float, T1: float = 300):
+        """
+        Solves for the initial pressure and incident shock velocity given the target
+        post-reflected-shock conditions.
+
+        Parameters:
+            thermo: Thermodynamic interface.
+            T5: Temperature behind the reflected shock [K].
+            P5: Pressure behind the reflected shock [Pa].
+            T1: Initial temperature [K].
+
+        Exceptions:
+            ConvergenceError: If the relative change in `u1`, `P1`, `T2`, and `P2`
+                is not below the [`rtol`][rgfrosh.shock.FrozenShock.rtol]
+                within [`max_iter`][rgfrosh.shock.FrozenShock.max_iter] iterations.
+
+        """
+
+        thermo.TP = T5, P5
+        h5 = thermo.enthalpy_mass
+        nu5 = 1 / thermo.density_mass
+
+        thermo.TP = T1, 101325
+        cp1 = thermo.cp_mass
+        R = GAS_CONSTANT / thermo.mean_molecular_weight
+        gamma1 = cp1 / (cp1 - R)
+        a1 = (gamma1 * GAS_CONSTANT / thermo.mean_molecular_weight * T1) ** 0.5
+
+        MS = IdealShock.incident_Mach_number(gamma1, T5, T1)
+        P1 = P5 / IdealShock.reflected_pressure_ratio(MS, gamma1)
+        P2 = P1 * IdealShock.incident_pressure_ratio(MS, gamma1)
+        T2 = T1 * IdealShock.incident_temperature_ratio(MS, gamma1)
+
+        u1 = MS * a1
+
+        for i in range(FrozenShock.max_iter):
+            thermo.TP = T1, P1
+            h1 = thermo.enthalpy_mass
+            nu1 = 1 / thermo.density_mass
+            beta1 = thermo.thermal_expansion_coeff
+            kappa1 = thermo.isothermal_compressibility
+
+            thermo.TP = T2, P2
+            h2 = thermo.enthalpy_mass
+            nu2 = 1 / thermo.density_mass
+            cp2 = thermo.cp_mass
+            beta2 = thermo.thermal_expansion_coeff
+            kappa2 = thermo.isothermal_compressibility
+
+            f1 = P2 / P1 - 1 + u1**2 / (P1 * nu1) * (nu2 / nu1 - 1)
+            f2 = 2 * (h2 - h1) / u1**2 + (nu2 / nu1) ** 2 - 1
+            f3 = (P5 / P2 - 1) + (u1 * (1 - nu2 / nu1)) ** 2 / P2 / (nu5 - nu2)
+            f4 = 2 * (h5 - h2) / (u1 * (1 - nu2 / nu1)) ** 2 + (nu5 + nu2) / (nu5 - nu2)
+
+            df1_du1 = 2 * u1 / (P1 * nu1**2) * (nu2 - nu1)
+            df1_dP1 = -P2 / P1**2 + u1**2 / (P1**2 * nu1**2) * (
+                P1 * kappa1 * (2 * nu2 - nu1) - (nu2 - nu1)
+            )
+            df1_dT2 = u1**2 * nu2 * beta2 / (P1 * nu1**2)
+            df1_dP2 = 1 / P1 - u1**2 * nu2 * kappa2 / (P1 * nu1**2)
+
+            df2_du1 = -4 * (h2 - h1) / u1**3
+            df2_dP1 = (
+                2 * nu2**2 * kappa1 / nu1**2 - 2 * nu1 * (1 - T1 * beta1) / u1**2
+            )
+            df2_dT2 = 2 * cp2 / u1**2 + 2 * (nu2 / nu1) ** 2 * beta2
+            df2_dP2 = (
+                2 * nu2 * (1 - T2 * beta2) / u1**2 - 2 * nu2**2 * kappa2 / nu1**2
+            )
+
+            df3_du1 = 2 * u1 * (1 - nu2 / nu1) ** 2 / (P2 * (nu5 - nu2))
+            df3_dP2 = -P5 / P2**2 - (
+                u1**2 / (nu1**2 * P2) * (nu1 - nu2) / (nu5 - nu2)
+            ) * (nu2 * kappa2 * (nu1 + nu2 - 2 * nu5) / (nu5 - nu2) + (nu1 - nu2) / P2)
+
+            df3_dT2 = (
+                (u1**2 * nu2 * beta2)
+                / (P2 * nu1**2)
+                * (nu1 - nu2)
+                / (nu5 - nu2) ** 2
+                * (nu1 + nu2 - 2 * nu5)
+            )
+            df4_dT2 = (2 * nu1**2 / u1**2) * (
+                2 * nu2 * beta2 * (h5 - h2) - cp2 * (nu1 - nu2)
+            ) / (nu1 - nu2) ** 3 + 2 * nu2 * nu5 * beta2 / (nu5 - nu2) ** 2
+            df4_dP2 = (-2 * nu1**2 * nu2) / u1**2 * (
+                2 * kappa2 * (h5 - h2) + (nu1 - nu2) * (1 - T2 * beta2)
+            ) / (nu1 - nu2) ** 3 - 2 * nu2 * nu5 * kappa2 / (nu5 - nu2) ** 2
+            df3_dP1 = (
+                -2 * u1**2 * nu2 * kappa1 * (1 - nu2 / nu1) / (P2 * nu1 * (nu5 - nu2))
+            )
+            df4_du1 = -4 * (h5 - h2) / (u1**3 * (1 - nu2 / nu1) ** 2)
+            df4_dP1 = (
+                4 * nu2 * kappa1 * (h5 - h2) / (u1**2 * nu1) / (1 - nu2 / nu1) ** 3
+            )
+
+            delta_u1, delta_P1, delta_T2, delta_P2 = np.matmul(
+                np.linalg.inv(
+                    np.array(
+                        [
+                            [df1_du1, df1_dP1, df1_dT2, df1_dP2],
+                            [df2_du1, df2_dP1, df2_dT2, df2_dP2],
+                            [df3_du1, df3_dP1, df3_dT2, df3_dP2],
+                            [df4_du1, df4_dP1, df4_dT2, df4_dP2],
+                        ]
+                    )
+                ),
+                np.array([f1, f2, f3, f4]),
+            )
+
+            converged = (
+                abs(delta_u1) <= u1 * FrozenShock.rtol
+                and abs(delta_P1) <= P1 * FrozenShock.rtol
+                and abs(delta_T2) <= T2 * FrozenShock.rtol
+                and abs(delta_P2) <= P2 * FrozenShock.rtol
+            )
+
+            u1 -= delta_u1
+            P1 -= delta_P1
+            T2 -= delta_T2
+            P2 -= delta_P2
+
+            if converged:
+                thermo.TP = T1, P1
+                rho1 = thermo.density_mass
+                thermo.TP = T2, P2
+                rho2 = thermo.density_mass
+
+                u2 = u1 * rho1 / rho2
+                u5 = (u1 - u2) / (nu2 / nu5 - 1)
+
+                return u1, P1, u2, T2, P2, u5
+
+        raise ConvergenceError
```

### Comparing `rgfrosh-0.2.0/rgfrosh.egg-info/PKG-INFO` & `rgfrosh-0.2.1/rgfrosh.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,96 +1,98 @@
-Metadata-Version: 2.1
-Name: rgfrosh
-Version: 0.2.0
-Summary: A frozen shock solver for ideal and real gas equations of state.
-Home-page: https://github.com/VasuLab/RGFROSH
-Author: Cory Kinney
-Author-email: corykinney@ucf.edu
-License: MIT
-Platform: any
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Python Real Gas FROzen SHock (RGFROSH)
-
-![CI](https://github.com/VasuLab/RGFROSH/actions/workflows/main.yml/badge.svg?event=push)
-[![codecov](https://codecov.io/gh/VasuLab/RGFROSH/branch/main/graph/badge.svg?token=00W4E78FDD)](https://codecov.io/gh/VasuLab/RGFROSH)
-[![pypi](https://img.shields.io/pypi/v/rgfrosh.svg)](https://pypi.python.org/pypi/rgfrosh)
-[![versions](https://img.shields.io/pypi/pyversions/rgfrosh.svg)](https://github.com/VasuLab/rgfrosh)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
-[![license](https://img.shields.io/github/license/VasuLab/rgfrosh.svg)](https://github.com/VasuLab/rgfrosh/blob/main/LICENSE)
-[![DOI](https://zenodo.org/badge/435992350.svg)](https://zenodo.org/badge/latestdoi/435992350)
-
-> This project is a solver for the frozen shock equations[^1] developed in Python at the
-> University of Central Florida. The original RGFROSH was developed in FORTRAN at Stanford 
-> University by D. F. Davidson and R. K. Hanson using real gas subroutines for 
-> CHEMKIN[^2][^3]. 
-
-Python RGFROSH (`rgfrosh`) is a package for calculating conditions behind incident and reflected shock in
-a shock tube for an arbitrary equation of state. 
-
-## Documentation
-
-The [documentation site](https://vasulab.github.io/RGFROSH) provides a detailed 
-[user guide](https://vasulab.github.io/RGFROSH/guide/getting-started) and 
-[reference](https://vasulab.github.io/RGFROSH/reference) for the package.
-
-## Installation
-
-Python RGFROSH can be installed using
-
-```
-pip install rgfrosh
-```
-
-which also installs required dependencies. Cantera or CoolProp are optional and must
-be installed separately if desired.
-
-## Contributing
-
-For any bugs or feature requests, create an issue on the 
-[issue tracker](https://github.com/VasuLab/RGFROSH/issues). 
-
-After cloning the repository, the development environment can be set up with
-
-```
-pip install -r requirements.txt
-```
-
-Before creating a pull request, be sure to lint
-
-```
-black .
-```
-
-and run the automated tests
-
-```
-pytest
-```
-
-These checks will be performed automatically for all pull requests along
-with test coverage comparisons.
-
-## Cite
-
-To cite Python RGFROSH click <kbd>Cite this repository</kbd>on the right side of the GitHub repository
-page to export the citation for the latest release of `rgfrosh`. It is also encouraged to cite the 
-original paper[^1] for the frozen shock equations that this work is a derived from.
-
-
-[^1]: Davidson, D.F. and Hanson, R.K. (1996), Real Gas Corrections in Shock Tube Studies 
-at High Pressures. Isr. J. Chem., 36: 321-326. https://doi.org/10.1002/ijch.199600044
-[^2]: P. Barry Butler, "Real Gas Equations of State for Chemkin" Sandia Report No. 
-SAND88-3188 (1988). https://doi.org/10.2172/6224858
-[^3]: R. G. Schmitt, P. B. Butler, N. B. French "Chemkin real gas: a Fortran package for 
-analaysis of thermodynamic properties and chemical kinetics in non-ideal systems," 
-U. of Iowa Report UIME PPB 93-006 (1994).
+Metadata-Version: 2.1
+Name: rgfrosh
+Version: 0.2.1
+Summary: A frozen shock solver for ideal and real gas equations of state.
+Home-page: https://github.com/VasuLab/RGFROSH
+Author: Cory Kinney
+Author-email: corykinney@ucf.edu
+License: MIT
+Platform: any
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Python Real Gas FROzen SHock (RGFROSH)
+
+![CI](https://github.com/VasuLab/RGFROSH/actions/workflows/main.yml/badge.svg?event=push)
+[![codecov](https://codecov.io/gh/VasuLab/RGFROSH/branch/main/graph/badge.svg?token=00W4E78FDD)](https://codecov.io/gh/VasuLab/RGFROSH)
+[![pypi](https://img.shields.io/pypi/v/rgfrosh.svg)](https://pypi.python.org/pypi/rgfrosh)
+[![versions](https://img.shields.io/pypi/pyversions/rgfrosh.svg)](https://github.com/VasuLab/rgfrosh)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+[![license](https://img.shields.io/github/license/VasuLab/rgfrosh.svg)](https://github.com/VasuLab/rgfrosh/blob/main/LICENSE)
+[![DOI](https://zenodo.org/badge/435992350.svg)](https://zenodo.org/badge/latestdoi/435992350)
+
+> This project is a solver for the frozen shock equations[^1] developed in Python at the
+> University of Central Florida. The original RGFROSH was developed in FORTRAN at Stanford 
+> University by D. F. Davidson and R. K. Hanson using real gas subroutines for 
+> CHEMKIN[^2][^3]. 
+
+Python RGFROSH (`rgfrosh`) is a package for calculating conditions behind incident and reflected shock in
+a shock tube. As its name suggests, `rgfrosh` was written primarily for solving the frozen shock equations for
+a real gas equation of state; however, the implementation also allows for the use of the ideal gas equation of state or 
+even custom equations of state. Additionally, an implementation of the ideal shock equations is also available for comparison. 
+
+## Documentation
+
+The [documentation site](https://vasulab.github.io/RGFROSH) provides a detailed 
+[user guide](https://vasulab.github.io/RGFROSH/guide/getting-started) and 
+[reference](https://vasulab.github.io/RGFROSH/reference) for the package.
+
+## Installation
+
+Python RGFROSH can be installed using
+
+```
+pip install rgfrosh
+```
+
+which also installs required dependencies. Cantera or CoolProp are optional and must
+be installed separately if desired.
+
+## Contributing
+
+For any bugs or feature requests, create an issue on the 
+[issue tracker](https://github.com/VasuLab/RGFROSH/issues). 
+
+After cloning the repository, the development environment can be set up with
+
+```
+pip install -r requirements.txt
+```
+
+Before creating a pull request, be sure to lint
+
+```
+black .
+```
+
+and run the automated tests
+
+```
+pytest
+```
+
+These checks will be performed automatically for all pull requests along
+with test coverage comparisons.
+
+## Cite
+
+To cite Python RGFROSH click <kbd>Cite this repository</kbd>on the right side of the GitHub repository
+page to export the citation for the latest release of `rgfrosh`. It is also encouraged to cite the 
+original paper[^1] for the frozen shock equations that this work is a derived from.
+
+
+[^1]: Davidson, D.F. and Hanson, R.K. (1996), Real Gas Corrections in Shock Tube Studies 
+at High Pressures. Isr. J. Chem., 36: 321-326. https://doi.org/10.1002/ijch.199600044
+[^2]: P. Barry Butler, "Real Gas Equations of State for Chemkin" Sandia Report No. 
+SAND88-3188 (1988). https://doi.org/10.2172/6224858
+[^3]: R. G. Schmitt, P. B. Butler, N. B. French "Chemkin real gas: a Fortran package for 
+analaysis of thermodynamic properties and chemical kinetics in non-ideal systems," 
+U. of Iowa Report UIME PPB 93-006 (1994).
```

### Comparing `rgfrosh-0.2.0/test/test_frozen_shock.py` & `rgfrosh-0.2.1/test/test_frozen_shock.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,192 +1,192 @@
-"""
-Tests for the `FrozenShock` class.
-"""
-
-from rgfrosh import ThermoInterface, IdealShock, FrozenShock
-from rgfrosh.thermo import CPInterface
-from rgfrosh.constants import GAS_CONSTANT
-
-import cantera as ct
-import CoolProp as CP
-
-from numpy.testing import assert_almost_equal, assert_allclose
-import pytest
-
-
-FrozenShock.rtol = 1e-9
-
-
-class PerfectGas(ThermoInterface):
-    """Thermo interface for a calorically perfect gas."""
-
-    def __init__(self, gamma, MW):
-        self._T = 300
-        self._P = 101325
-        self.gamma = gamma
-        self.MW = MW
-
-    @property
-    def TP(self):
-        return self._T, self._P
-
-    @TP.setter
-    def TP(self, value):
-        self._T, self._P = value
-
-    @property
-    def mean_molecular_weight(self):
-        return self.MW
-
-    @property
-    def density_mass(self):
-        return self._P / (GAS_CONSTANT / self.MW * self._T)
-
-    @property
-    def cp_mass(self):
-        return self.gamma / (self.gamma - 1) * GAS_CONSTANT / self.MW
-
-    @property
-    def enthalpy_mass(self):
-        return self.cp_mass * self._T
-
-    @property
-    def isothermal_compressibility(self):
-        return 1 / self._P
-
-    @property
-    def thermal_expansion_coeff(self):
-        return 1 / self._T
-
-    @property
-    def sound_speed(self):
-        return (self.gamma * GAS_CONSTANT / self.MW * self._T) ** 0.5
-
-
-@pytest.mark.parametrize("gamma,MW", [(7 / 5, 28), (5 / 3, 40)])  # [Nitrogen, Argon]
-@pytest.mark.parametrize("M", [1.5, 2, 2.5, 3, 3.5, 4, 4.5, 5])
-class TestIdealCase:
-    """
-    Tests that the `FrozenShock` implementation correctly reduces to the ideal shock equations[^1]
-    for the case of a calorically perfect gas `ThermoInterface`.
-
-    [^1]: Gaydon, A. G. and I. R. Hurle (1963). The shock tube in high-temperature chemical physics.
-    """
-
-    @pytest.fixture
-    def ideal_case(self, M, gamma, MW):
-        perfect_gas = PerfectGas(gamma, MW)
-        return FrozenShock(
-            perfect_gas, u1=M * perfect_gas.sound_speed, T1=300, P1=101325
-        )
-
-    def test_incident_temperature_ratio(self, ideal_case, M, gamma, MW):
-        assert_almost_equal(
-            ideal_case.T2 / ideal_case.T1,
-            IdealShock.incident_temperature_ratio(M, gamma),
-        )
-
-    def test_incident_pressure_ratio(self, ideal_case, M, gamma, MW):
-        assert_almost_equal(
-            ideal_case.P2 / ideal_case.P1,
-            IdealShock.incident_pressure_ratio(M, gamma),
-        )
-
-    def test_incident_density_ratio(self, ideal_case, M, gamma, MW):
-        assert_almost_equal(
-            ideal_case.rho2 / ideal_case.rho1,
-            IdealShock.incident_density_ratio(M, gamma),
-        )
-
-    def test_incident_velocity_ratio(self, ideal_case, M, gamma, MW):
-        assert_almost_equal(
-            ideal_case.u1 / ideal_case.u2,
-            IdealShock.incident_density_ratio(M, gamma),
-        )
-
-    def test_reflected_temperature_ratio(self, ideal_case, M, gamma, MW):
-        assert_almost_equal(
-            ideal_case.T5 / ideal_case.T1,
-            IdealShock.reflected_temperature_ratio(M, gamma),
-        )
-
-    def test_reflected_pressure_ratio(self, ideal_case, M, gamma, MW):
-        assert_almost_equal(
-            ideal_case.P5 / ideal_case.P1,
-            IdealShock.reflected_pressure_ratio(M, gamma),
-        )
-
-    @pytest.mark.xfail
-    def test_reflected_velocity_ratio(self, ideal_case, M, gamma, MW):
-        assert_almost_equal(
-            ideal_case.u5 / ideal_case.u1,
-            IdealShock.reflected_velocity_ratio(M, gamma),
-        )
-
-
-class TestRealGas:
-    """
-    Test FrozenShock output against output of the original RGFROSH[^2] for the
-    Peng-Robinson EOS for nitrogen (from table in the addendum).
-
-    [^2]: Davidson, D. F. and R. K. Hanson (1996). "Real Gas Corrections in Shock Tube
-    Studies at High Pressures." Israel Journal of Chemistry 36(3): 321-326.
-    """
-
-    data = [
-        (762, 1, 814.9, 19.95, 8.303),
-        (762, 10, 809.0, 197.37, 78.143),
-        (1000, 1, 1208.4, 45.56, 12.732),
-        (1000, 10, 1191.9, 450.47, 116.194),
-        (1523, 1, 2338, 145.0, 20.817),
-        (1523, 10, 2286, 1432, 181.60),
-    ]
-
-    @staticmethod
-    @pytest.fixture
-    def gas():
-        state = CP.AbstractState("PR", "Nitrogen")
-        state.specify_phase(CP.iphase_supercritical_gas)
-        return CPInterface(state)
-
-    @staticmethod
-    @pytest.mark.parametrize("u1,P1,T5,P5,rho5", data)
-    def test_reflected_conditions(gas, u1, P1, T5, P5, rho5):
-        shock = FrozenShock(gas, u1=u1, T1=293, P1=P1 * 101325)
-        assert_allclose(
-            [shock.T5, shock.P5 / 101325, shock.rho5],
-            [T5, P5, rho5],
-            rtol=1e-3,
-        )
-
-
-@pytest.mark.parametrize("gas", [ct.Nitrogen(), ct.CarbonDioxide()])
-@pytest.mark.parametrize("u1", [400, 450, 500, 550, 600, 650, 700, 750, 800])
-def test_consistency(gas, u1):
-    """
-    Tests for consistency between the initialization approaches using the following steps:
-
-    1. Initialize a `FrozenShock` object using `M`, `T1`, and `P1`
-    2. Initialize another `FrozenShock` object using the calculated `T5` and `P5` from step 1
-    3. Check that all properties are consistent between the objects from steps 1 and 2
-    """
-
-    gas = ct.Nitrogen()
-    from_initial = FrozenShock(gas, u1=u1, T1=300, P1=101325)
-    from_target = FrozenShock(
-        gas, T5=from_initial.T5, P5=from_initial.P5, T1=from_initial.T1
-    )
-
-    assert_allclose(from_initial.u1, from_target.u1)
-    assert_allclose(from_initial.T1, from_target.T1)
-    assert_allclose(from_initial.P1, from_target.P1)
-    assert_allclose(from_initial.rho1, from_target.rho1)
-
-    assert_allclose(from_initial.u2, from_target.u2)
-    assert_allclose(from_initial.T2, from_target.T2)
-    assert_allclose(from_initial.P2, from_target.P2)
-    assert_allclose(from_initial.rho2, from_target.rho2)
-
-    assert_allclose(from_initial.u5, from_target.u5)
-    assert_allclose(from_initial.T5, from_target.T5)
-    assert_allclose(from_initial.P5, from_target.P5)
-    assert_allclose(from_initial.rho5, from_target.rho5)
+"""
+Tests for the `FrozenShock` class.
+"""
+
+from rgfrosh import ThermoInterface, IdealShock, FrozenShock
+from rgfrosh.thermo import CPInterface
+from rgfrosh.constants import GAS_CONSTANT
+
+import cantera as ct
+import CoolProp as CP
+
+from numpy.testing import assert_almost_equal, assert_allclose
+import pytest
+
+
+FrozenShock.rtol = 1e-9
+
+
+class PerfectGas(ThermoInterface):
+    """Thermo interface for a calorically perfect gas."""
+
+    def __init__(self, gamma, MW):
+        self._T = 300
+        self._P = 101325
+        self.gamma = gamma
+        self.MW = MW
+
+    @property
+    def TP(self):
+        return self._T, self._P
+
+    @TP.setter
+    def TP(self, value):
+        self._T, self._P = value
+
+    @property
+    def mean_molecular_weight(self):
+        return self.MW
+
+    @property
+    def density_mass(self):
+        return self._P / (GAS_CONSTANT / self.MW * self._T)
+
+    @property
+    def cp_mass(self):
+        return self.gamma / (self.gamma - 1) * GAS_CONSTANT / self.MW
+
+    @property
+    def enthalpy_mass(self):
+        return self.cp_mass * self._T
+
+    @property
+    def isothermal_compressibility(self):
+        return 1 / self._P
+
+    @property
+    def thermal_expansion_coeff(self):
+        return 1 / self._T
+
+    @property
+    def sound_speed(self):
+        return (self.gamma * GAS_CONSTANT / self.MW * self._T) ** 0.5
+
+
+@pytest.mark.parametrize("gamma,MW", [(7 / 5, 28), (5 / 3, 40)])  # [Nitrogen, Argon]
+@pytest.mark.parametrize("M", [1.5, 2, 2.5, 3, 3.5, 4, 4.5, 5])
+class TestIdealCase:
+    """
+    Tests that the `FrozenShock` implementation correctly reduces to the ideal shock equations[^1]
+    for the case of a calorically perfect gas `ThermoInterface`.
+
+    [^1]: Gaydon, A. G. and I. R. Hurle (1963). The shock tube in high-temperature chemical physics.
+    """
+
+    @pytest.fixture
+    def ideal_case(self, M, gamma, MW):
+        perfect_gas = PerfectGas(gamma, MW)
+        return FrozenShock(
+            perfect_gas, u1=M * perfect_gas.sound_speed, T1=300, P1=101325
+        )
+
+    def test_incident_temperature_ratio(self, ideal_case, M, gamma, MW):
+        assert_almost_equal(
+            ideal_case.T2 / ideal_case.T1,
+            IdealShock.incident_temperature_ratio(M, gamma),
+        )
+
+    def test_incident_pressure_ratio(self, ideal_case, M, gamma, MW):
+        assert_almost_equal(
+            ideal_case.P2 / ideal_case.P1,
+            IdealShock.incident_pressure_ratio(M, gamma),
+        )
+
+    def test_incident_density_ratio(self, ideal_case, M, gamma, MW):
+        assert_almost_equal(
+            ideal_case.rho2 / ideal_case.rho1,
+            IdealShock.incident_density_ratio(M, gamma),
+        )
+
+    def test_incident_velocity_ratio(self, ideal_case, M, gamma, MW):
+        assert_almost_equal(
+            ideal_case.u1 / ideal_case.u2,
+            IdealShock.incident_density_ratio(M, gamma),
+        )
+
+    def test_reflected_temperature_ratio(self, ideal_case, M, gamma, MW):
+        assert_almost_equal(
+            ideal_case.T5 / ideal_case.T1,
+            IdealShock.reflected_temperature_ratio(M, gamma),
+        )
+
+    def test_reflected_pressure_ratio(self, ideal_case, M, gamma, MW):
+        assert_almost_equal(
+            ideal_case.P5 / ideal_case.P1,
+            IdealShock.reflected_pressure_ratio(M, gamma),
+        )
+
+    @pytest.mark.xfail
+    def test_reflected_velocity_ratio(self, ideal_case, M, gamma, MW):
+        assert_almost_equal(
+            ideal_case.u5 / ideal_case.u1,
+            IdealShock.reflected_velocity_ratio(M, gamma),
+        )
+
+
+class TestRealGas:
+    """
+    Test FrozenShock output against output of the original RGFROSH[^2] for the
+    Peng-Robinson EOS for nitrogen (from table in the addendum).
+
+    [^2]: Davidson, D. F. and R. K. Hanson (1996). "Real Gas Corrections in Shock Tube
+    Studies at High Pressures." Israel Journal of Chemistry 36(3): 321-326.
+    """
+
+    data = [
+        (762, 1, 814.9, 19.95, 8.303),
+        (762, 10, 809.0, 197.37, 78.143),
+        (1000, 1, 1208.4, 45.56, 12.732),
+        (1000, 10, 1191.9, 450.47, 116.194),
+        (1523, 1, 2338, 145.0, 20.817),
+        (1523, 10, 2286, 1432, 181.60),
+    ]
+
+    @staticmethod
+    @pytest.fixture
+    def gas():
+        state = CP.AbstractState("PR", "Nitrogen")
+        state.specify_phase(CP.iphase_supercritical_gas)
+        return CPInterface(state)
+
+    @staticmethod
+    @pytest.mark.parametrize("u1,P1,T5,P5,rho5", data)
+    def test_reflected_conditions(gas, u1, P1, T5, P5, rho5):
+        shock = FrozenShock(gas, u1=u1, T1=293, P1=P1 * 101325)
+        assert_allclose(
+            [shock.T5, shock.P5 / 101325, shock.rho5],
+            [T5, P5, rho5],
+            rtol=1e-3,
+        )
+
+
+@pytest.mark.parametrize("gas", [ct.Nitrogen(), ct.CarbonDioxide()])
+@pytest.mark.parametrize("u1", [400, 450, 500, 550, 600, 650, 700, 750, 800])
+def test_consistency(gas, u1):
+    """
+    Tests for consistency between the initialization approaches using the following steps:
+
+    1. Initialize a `FrozenShock` object using `M`, `T1`, and `P1`
+    2. Initialize another `FrozenShock` object using the calculated `T5` and `P5` from step 1
+    3. Check that all properties are consistent between the objects from steps 1 and 2
+    """
+
+    gas = ct.Nitrogen()
+    from_initial = FrozenShock(gas, u1=u1, T1=300, P1=101325)
+    from_target = FrozenShock(
+        gas, T5=from_initial.T5, P5=from_initial.P5, T1=from_initial.T1
+    )
+
+    assert_allclose(from_initial.u1, from_target.u1)
+    assert_allclose(from_initial.T1, from_target.T1)
+    assert_allclose(from_initial.P1, from_target.P1)
+    assert_allclose(from_initial.rho1, from_target.rho1)
+
+    assert_allclose(from_initial.u2, from_target.u2)
+    assert_allclose(from_initial.T2, from_target.T2)
+    assert_allclose(from_initial.P2, from_target.P2)
+    assert_allclose(from_initial.rho2, from_target.rho2)
+
+    assert_allclose(from_initial.u5, from_target.u5)
+    assert_allclose(from_initial.T5, from_target.T5)
+    assert_allclose(from_initial.P5, from_target.P5)
+    assert_allclose(from_initial.rho5, from_target.rho5)
```

### Comparing `rgfrosh-0.2.0/test/test_ideal_shock.py` & `rgfrosh-0.2.1/test/test_ideal_shock.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,141 +1,141 @@
-"""
-Tests for the `IdealShock` class.
-"""
-
-from rgfrosh import IdealShock
-
-from numpy.testing import assert_allclose
-import pytest
-
-
-class TestRatios:
-    r"""
-    Test `IdealShock` against values derived from example calculations in Table II.3 of
-    Gaydon and Hurle [^1].
-
-    [^1]: Gaydon, A. G. and I. R. Hurle (1963). The shock tube in high-temperature chemical
-    physics, Reinhold Publishing Corporation.
-    """
-
-    rtol = 0.5e-2
-
-    @staticmethod
-    @pytest.mark.parametrize(
-        ("gamma", "M1", "P2_1"),
-        [(7 / 5, 2.95, 10), (7 / 5, 6.56, 50), (5 / 3, 2.87, 10), (5 / 3, 6.34, 50)],
-    )
-    def test_incident_pressure_ratio(gamma, M1, P2_1):
-        assert_allclose(
-            IdealShock.incident_pressure_ratio(M1, gamma), P2_1, rtol=TestRatios.rtol
-        )
-
-    @staticmethod
-    @pytest.mark.parametrize(
-        ("gamma", "M1", "T2_1"),
-        [
-            (7 / 5, 2.95, 2.62),
-            (7 / 5, 6.56, 9.31),
-            (5 / 3, 2.87, 3.42),
-            (5 / 3, 6.34, 13.4),
-        ],
-    )
-    def test_incident_temperature_ratio(gamma, M1, T2_1):
-        assert_allclose(
-            IdealShock.incident_temperature_ratio(M1, gamma), T2_1, rtol=TestRatios.rtol
-        )
-
-    @staticmethod
-    @pytest.mark.parametrize(
-        ("gamma", "M1", "rho2_1"),
-        [
-            (7 / 5, 2.95, 3.82),
-            (7 / 5, 6.56, 5.37),
-            (5 / 3, 2.87, 2.92),
-            (5 / 3, 6.34, 3.72),
-        ],
-    )
-    def test_incident_density_ratio(gamma, M1, rho2_1):
-        assert_allclose(
-            IdealShock.incident_density_ratio(M1, gamma), rho2_1, rtol=TestRatios.rtol
-        )
-
-    @staticmethod
-    @pytest.mark.parametrize(
-        ("gamma", "M1", "P2_1", "P5_2"),
-        [
-            (7 / 5, 2.95, 10, 4.95),
-            (7 / 5, 6.56, 50, 7.12),
-            (5 / 3, 2.87, 10, 4.22),
-            (5 / 3, 6.34, 50, 5.54),
-        ],
-    )
-    def test_reflected_pressure_ratio(gamma, M1, P2_1, P5_2):
-        assert_allclose(
-            IdealShock.reflected_pressure_ratio(M1, gamma),
-            P5_2 * P2_1,
-            rtol=TestRatios.rtol,
-        )
-
-    @staticmethod
-    @pytest.mark.parametrize(
-        ("gamma", "M1", "T2_1", "T5_2"),
-        [
-            (7 / 5, 2.95, 2.62, 1.76),
-            pytest.param(7 / 5, 6.56, 9.31, 2.28, marks=pytest.mark.xfail),
-            (5 / 3, 2.87, 3.42, 1.94),
-            pytest.param(5 / 3, 6.34, 13.4, 2.37, marks=pytest.mark.xfail),
-        ],
-    )
-    def test_reflected_temperature_ratio(gamma, M1, T2_1, T5_2):
-        assert_allclose(
-            IdealShock.reflected_temperature_ratio(M1, gamma),
-            T5_2 * T2_1,
-            rtol=TestRatios.rtol,
-        )
-
-    @staticmethod
-    @pytest.mark.parametrize(
-        ("gamma", "M1", "VR_S"),
-        [
-            (7 / 5, 2.95, 0.423),
-            (7 / 5, 6.56, 0.351),
-            (5 / 3, 2.87, 0.589),
-            (5 / 3, 6.34, 0.517),
-        ],
-    )
-    def test_reflected_velocity_ratio(gamma, M1, VR_S):
-        assert_allclose(
-            IdealShock.reflected_velocity_ratio(M1, gamma), VR_S, rtol=TestRatios.rtol
-        )
-
-
-@pytest.mark.parametrize("gamma,MW", [(7 / 5, 28), (5 / 3, 40)])  # [Nitrogen, Argon]
-@pytest.mark.parametrize("M", [1.5, 2, 2.5, 3, 3.5, 4, 4.5, 5])
-def test_consistency(gamma, MW, M):
-    """
-    Tests for consistency between the initialization approaches using the following steps:
-
-    1. Initialize an `IdealShock` object using `M`, `T1`, and `P1`
-    2. Initialize another `IdealShock` object using the calculated `T5` and `P5` from step 1
-    3. Check that all properties are consistent between the objects from steps 1 and 2
-    """
-
-    from_initial = IdealShock(gamma, MW, M=M, T1=300, P1=101325)
-    from_target = IdealShock(
-        gamma, MW, T5=from_initial.T5, P5=from_initial.P5, T1=from_initial.T1
-    )
-
-    assert_allclose(from_initial.u1, from_target.u1)
-    assert_allclose(from_initial.T1, from_target.T1)
-    assert_allclose(from_initial.P1, from_target.P1)
-    assert_allclose(from_initial.rho1, from_target.rho1)
-
-    assert_allclose(from_initial.u2, from_target.u2)
-    assert_allclose(from_initial.T2, from_target.T2)
-    assert_allclose(from_initial.P2, from_target.P2)
-    assert_allclose(from_initial.rho2, from_target.rho2)
-
-    assert_allclose(from_initial.u5, from_target.u5)
-    assert_allclose(from_initial.T5, from_target.T5)
-    assert_allclose(from_initial.P5, from_target.P5)
-    assert_allclose(from_initial.rho5, from_target.rho5)
+"""
+Tests for the `IdealShock` class.
+"""
+
+from rgfrosh import IdealShock
+
+from numpy.testing import assert_allclose
+import pytest
+
+
+class TestRatios:
+    r"""
+    Test `IdealShock` against values derived from example calculations in Table II.3 of
+    Gaydon and Hurle [^1].
+
+    [^1]: Gaydon, A. G. and I. R. Hurle (1963). The shock tube in high-temperature chemical
+    physics, Reinhold Publishing Corporation.
+    """
+
+    rtol = 0.5e-2
+
+    @staticmethod
+    @pytest.mark.parametrize(
+        ("gamma", "M1", "P2_1"),
+        [(7 / 5, 2.95, 10), (7 / 5, 6.56, 50), (5 / 3, 2.87, 10), (5 / 3, 6.34, 50)],
+    )
+    def test_incident_pressure_ratio(gamma, M1, P2_1):
+        assert_allclose(
+            IdealShock.incident_pressure_ratio(M1, gamma), P2_1, rtol=TestRatios.rtol
+        )
+
+    @staticmethod
+    @pytest.mark.parametrize(
+        ("gamma", "M1", "T2_1"),
+        [
+            (7 / 5, 2.95, 2.62),
+            (7 / 5, 6.56, 9.31),
+            (5 / 3, 2.87, 3.42),
+            (5 / 3, 6.34, 13.4),
+        ],
+    )
+    def test_incident_temperature_ratio(gamma, M1, T2_1):
+        assert_allclose(
+            IdealShock.incident_temperature_ratio(M1, gamma), T2_1, rtol=TestRatios.rtol
+        )
+
+    @staticmethod
+    @pytest.mark.parametrize(
+        ("gamma", "M1", "rho2_1"),
+        [
+            (7 / 5, 2.95, 3.82),
+            (7 / 5, 6.56, 5.37),
+            (5 / 3, 2.87, 2.92),
+            (5 / 3, 6.34, 3.72),
+        ],
+    )
+    def test_incident_density_ratio(gamma, M1, rho2_1):
+        assert_allclose(
+            IdealShock.incident_density_ratio(M1, gamma), rho2_1, rtol=TestRatios.rtol
+        )
+
+    @staticmethod
+    @pytest.mark.parametrize(
+        ("gamma", "M1", "P2_1", "P5_2"),
+        [
+            (7 / 5, 2.95, 10, 4.95),
+            (7 / 5, 6.56, 50, 7.12),
+            (5 / 3, 2.87, 10, 4.22),
+            (5 / 3, 6.34, 50, 5.54),
+        ],
+    )
+    def test_reflected_pressure_ratio(gamma, M1, P2_1, P5_2):
+        assert_allclose(
+            IdealShock.reflected_pressure_ratio(M1, gamma),
+            P5_2 * P2_1,
+            rtol=TestRatios.rtol,
+        )
+
+    @staticmethod
+    @pytest.mark.parametrize(
+        ("gamma", "M1", "T2_1", "T5_2"),
+        [
+            (7 / 5, 2.95, 2.62, 1.76),
+            pytest.param(7 / 5, 6.56, 9.31, 2.28, marks=pytest.mark.xfail),
+            (5 / 3, 2.87, 3.42, 1.94),
+            pytest.param(5 / 3, 6.34, 13.4, 2.37, marks=pytest.mark.xfail),
+        ],
+    )
+    def test_reflected_temperature_ratio(gamma, M1, T2_1, T5_2):
+        assert_allclose(
+            IdealShock.reflected_temperature_ratio(M1, gamma),
+            T5_2 * T2_1,
+            rtol=TestRatios.rtol,
+        )
+
+    @staticmethod
+    @pytest.mark.parametrize(
+        ("gamma", "M1", "VR_S"),
+        [
+            (7 / 5, 2.95, 0.423),
+            (7 / 5, 6.56, 0.351),
+            (5 / 3, 2.87, 0.589),
+            (5 / 3, 6.34, 0.517),
+        ],
+    )
+    def test_reflected_velocity_ratio(gamma, M1, VR_S):
+        assert_allclose(
+            IdealShock.reflected_velocity_ratio(M1, gamma), VR_S, rtol=TestRatios.rtol
+        )
+
+
+@pytest.mark.parametrize("gamma,MW", [(7 / 5, 28), (5 / 3, 40)])  # [Nitrogen, Argon]
+@pytest.mark.parametrize("M", [1.5, 2, 2.5, 3, 3.5, 4, 4.5, 5])
+def test_consistency(gamma, MW, M):
+    """
+    Tests for consistency between the initialization approaches using the following steps:
+
+    1. Initialize an `IdealShock` object using `M`, `T1`, and `P1`
+    2. Initialize another `IdealShock` object using the calculated `T5` and `P5` from step 1
+    3. Check that all properties are consistent between the objects from steps 1 and 2
+    """
+
+    from_initial = IdealShock(gamma, MW, M=M, T1=300, P1=101325)
+    from_target = IdealShock(
+        gamma, MW, T5=from_initial.T5, P5=from_initial.P5, T1=from_initial.T1
+    )
+
+    assert_allclose(from_initial.u1, from_target.u1)
+    assert_allclose(from_initial.T1, from_target.T1)
+    assert_allclose(from_initial.P1, from_target.P1)
+    assert_allclose(from_initial.rho1, from_target.rho1)
+
+    assert_allclose(from_initial.u2, from_target.u2)
+    assert_allclose(from_initial.T2, from_target.T2)
+    assert_allclose(from_initial.P2, from_target.P2)
+    assert_allclose(from_initial.rho2, from_target.rho2)
+
+    assert_allclose(from_initial.u5, from_target.u5)
+    assert_allclose(from_initial.T5, from_target.T5)
+    assert_allclose(from_initial.P5, from_target.P5)
+    assert_allclose(from_initial.rho5, from_target.rho5)
```

