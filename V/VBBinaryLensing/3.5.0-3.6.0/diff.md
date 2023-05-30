# Comparing `tmp/VBBinaryLensing-3.5.0.tar.gz` & `tmp/VBBinaryLensing-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VBBinaryLensing-3.5.0.tar", last modified: Mon Feb 27 18:17:50 2023, max compression
+gzip compressed data, was "VBBinaryLensing-3.6.0.tar", last modified: Tue May 30 17:06:59 2023, max compression
```

## Comparing `VBBinaryLensing-3.5.0.tar` & `VBBinaryLensing-3.6.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 bachelet  (1000) bachelet  (1000)        0 2023-02-27 18:17:50.626831 VBBinaryLensing-3.5.0/
--rw-rw-r--   0 bachelet  (1000) bachelet  (1000)     7651 2023-02-27 16:56:06.000000 VBBinaryLensing-3.5.0/LICENSE
--rw-rw-r--   0 bachelet  (1000) bachelet  (1000)       59 2023-02-27 16:56:06.000000 VBBinaryLensing-3.5.0/MANIFEST.in
--rw-rw-r--   0 bachelet  (1000) bachelet  (1000)      399 2023-02-27 18:17:50.626831 VBBinaryLensing-3.5.0/PKG-INFO
--rw-rw-r--   0 bachelet  (1000) bachelet  (1000)     4046 2023-02-27 16:56:06.000000 VBBinaryLensing-3.5.0/README.md
-drwxrwxr-x   0 bachelet  (1000) bachelet  (1000)        0 2023-02-27 18:17:50.622831 VBBinaryLensing-3.5.0/VBBinaryLensing/
-drwxrwxr-x   0 bachelet  (1000) bachelet  (1000)        0 2023-02-27 18:17:50.622831 VBBinaryLensing-3.5.0/VBBinaryLensing/data/
--rw-rw-r--   0 bachelet  (1000) bachelet  (1000)   488032 2023-02-27 18:00:18.000000 VBBinaryLensing-3.5.0/VBBinaryLensing/data/ESPL.tbl
--rw-rw-r--   0 bachelet  (1000) bachelet  (1000)       18 2017-10-23 22:54:22.000000 VBBinaryLensing-3.5.0/VBBinaryLensing/data/OB151212coords.txt
--rw-rw-r--   0 bachelet  (1000) bachelet  (1000)        0 2023-02-27 16:56:06.000000 VBBinaryLensing-3.5.0/VBBinaryLensing/data/__init__.py
--rw-rw-r--   0 bachelet  (1000) bachelet  (1000)   110290 2016-06-24 20:05:36.000000 VBBinaryLensing-3.5.0/VBBinaryLensing/data/satellite1.txt
--rw-rw-r--   0 bachelet  (1000) bachelet  (1000)   112560 2016-06-24 20:06:10.000000 VBBinaryLensing-3.5.0/VBBinaryLensing/data/satellite2.txt
-drwxrwxr-x   0 bachelet  (1000) bachelet  (1000)        0 2023-02-27 18:17:50.626831 VBBinaryLensing-3.5.0/VBBinaryLensing/lib/
--rw-rw-r--   0 bachelet  (1000) bachelet  (1000)   144801 2023-02-27 18:00:18.000000 VBBinaryLensing-3.5.0/VBBinaryLensing/lib/VBBinaryLensingLibrary.cpp
--rw-rw-r--   0 bachelet  (1000) bachelet  (1000)    11101 2023-02-27 18:00:18.000000 VBBinaryLensing-3.5.0/VBBinaryLensing/lib/VBBinaryLensingLibrary.h
--rw-rw-r--   0 bachelet  (1000) bachelet  (1000)    30353 2023-02-27 16:56:06.000000 VBBinaryLensing-3.5.0/VBBinaryLensing/lib/python_bindings.cpp
-drwxrwxr-x   0 bachelet  (1000) bachelet  (1000)        0 2023-02-27 18:17:50.622831 VBBinaryLensing-3.5.0/VBBinaryLensing.egg-info/
--rw-rw-r--   0 bachelet  (1000) bachelet  (1000)      399 2023-02-27 18:17:50.000000 VBBinaryLensing-3.5.0/VBBinaryLensing.egg-info/PKG-INFO
--rw-rw-r--   0 bachelet  (1000) bachelet  (1000)      587 2023-02-27 18:17:50.000000 VBBinaryLensing-3.5.0/VBBinaryLensing.egg-info/SOURCES.txt
--rw-rw-r--   0 bachelet  (1000) bachelet  (1000)        1 2023-02-27 18:17:50.000000 VBBinaryLensing-3.5.0/VBBinaryLensing.egg-info/dependency_links.txt
--rw-rw-r--   0 bachelet  (1000) bachelet  (1000)        1 2023-02-27 18:17:50.000000 VBBinaryLensing-3.5.0/VBBinaryLensing.egg-info/not-zip-safe
--rw-rw-r--   0 bachelet  (1000) bachelet  (1000)       14 2023-02-27 18:17:50.000000 VBBinaryLensing-3.5.0/VBBinaryLensing.egg-info/requires.txt
--rw-rw-r--   0 bachelet  (1000) bachelet  (1000)       16 2023-02-27 18:17:50.000000 VBBinaryLensing-3.5.0/VBBinaryLensing.egg-info/top_level.txt
--rw-rw-r--   0 bachelet  (1000) bachelet  (1000)      875 2023-02-27 18:17:50.626831 VBBinaryLensing-3.5.0/setup.cfg
--rw-rw-r--   0 bachelet  (1000) bachelet  (1000)     3696 2023-02-27 18:00:18.000000 VBBinaryLensing-3.5.0/setup.py
+drwxrwxr-x   0 bachelet  (1000) bachelet  (1000)        0 2023-05-30 17:06:59.115445 VBBinaryLensing-3.6.0/
+-rw-rw-r--   0 bachelet  (1000) bachelet  (1000)     7651 2023-05-30 16:02:34.000000 VBBinaryLensing-3.6.0/LICENSE
+-rw-rw-r--   0 bachelet  (1000) bachelet  (1000)       59 2023-05-30 16:02:34.000000 VBBinaryLensing-3.6.0/MANIFEST.in
+-rw-rw-r--   0 bachelet  (1000) bachelet  (1000)      399 2023-05-30 17:06:59.115445 VBBinaryLensing-3.6.0/PKG-INFO
+-rw-rw-r--   0 bachelet  (1000) bachelet  (1000)     5143 2023-05-30 16:02:34.000000 VBBinaryLensing-3.6.0/README.md
+drwxrwxr-x   0 bachelet  (1000) bachelet  (1000)        0 2023-05-30 17:06:59.111445 VBBinaryLensing-3.6.0/VBBinaryLensing/
+drwxrwxr-x   0 bachelet  (1000) bachelet  (1000)        0 2023-05-30 17:06:59.115445 VBBinaryLensing-3.6.0/VBBinaryLensing/data/
+-rw-rw-r--   0 bachelet  (1000) bachelet  (1000)   488032 2023-05-30 16:02:34.000000 VBBinaryLensing-3.6.0/VBBinaryLensing/data/ESPL.tbl
+-rw-rw-r--   0 bachelet  (1000) bachelet  (1000)       18 2023-05-30 16:02:34.000000 VBBinaryLensing-3.6.0/VBBinaryLensing/data/OB151212coords.txt
+-rw-rw-r--   0 bachelet  (1000) bachelet  (1000)        0 2023-05-30 16:02:34.000000 VBBinaryLensing-3.6.0/VBBinaryLensing/data/__init__.py
+-rw-rw-r--   0 bachelet  (1000) bachelet  (1000)   110290 2023-05-30 16:02:34.000000 VBBinaryLensing-3.6.0/VBBinaryLensing/data/satellite1.txt
+-rw-rw-r--   0 bachelet  (1000) bachelet  (1000)   112560 2023-05-30 16:02:34.000000 VBBinaryLensing-3.6.0/VBBinaryLensing/data/satellite2.txt
+drwxrwxr-x   0 bachelet  (1000) bachelet  (1000)        0 2023-05-30 17:06:59.115445 VBBinaryLensing-3.6.0/VBBinaryLensing/lib/
+-rw-rw-r--   0 bachelet  (1000) bachelet  (1000)   145025 2023-05-30 16:55:13.000000 VBBinaryLensing-3.6.0/VBBinaryLensing/lib/VBBinaryLensingLibrary.cpp
+-rw-rw-r--   0 bachelet  (1000) bachelet  (1000)    11092 2023-05-30 16:55:13.000000 VBBinaryLensing-3.6.0/VBBinaryLensing/lib/VBBinaryLensingLibrary.h
+-rw-rw-r--   0 bachelet  (1000) bachelet  (1000)    30353 2023-05-30 16:02:34.000000 VBBinaryLensing-3.6.0/VBBinaryLensing/lib/python_bindings.cpp
+drwxrwxr-x   0 bachelet  (1000) bachelet  (1000)        0 2023-05-30 17:06:59.115445 VBBinaryLensing-3.6.0/VBBinaryLensing.egg-info/
+-rw-rw-r--   0 bachelet  (1000) bachelet  (1000)      399 2023-05-30 17:06:59.000000 VBBinaryLensing-3.6.0/VBBinaryLensing.egg-info/PKG-INFO
+-rw-rw-r--   0 bachelet  (1000) bachelet  (1000)      587 2023-05-30 17:06:59.000000 VBBinaryLensing-3.6.0/VBBinaryLensing.egg-info/SOURCES.txt
+-rw-rw-r--   0 bachelet  (1000) bachelet  (1000)        1 2023-05-30 17:06:59.000000 VBBinaryLensing-3.6.0/VBBinaryLensing.egg-info/dependency_links.txt
+-rw-rw-r--   0 bachelet  (1000) bachelet  (1000)        1 2023-05-30 16:08:24.000000 VBBinaryLensing-3.6.0/VBBinaryLensing.egg-info/not-zip-safe
+-rw-rw-r--   0 bachelet  (1000) bachelet  (1000)       14 2023-05-30 17:06:59.000000 VBBinaryLensing-3.6.0/VBBinaryLensing.egg-info/requires.txt
+-rw-rw-r--   0 bachelet  (1000) bachelet  (1000)       16 2023-05-30 17:06:59.000000 VBBinaryLensing-3.6.0/VBBinaryLensing.egg-info/top_level.txt
+-rw-rw-r--   0 bachelet  (1000) bachelet  (1000)      875 2023-05-30 17:06:59.115445 VBBinaryLensing-3.6.0/setup.cfg
+-rw-rw-r--   0 bachelet  (1000) bachelet  (1000)     3696 2023-05-30 16:55:13.000000 VBBinaryLensing-3.6.0/setup.py
```

### Comparing `VBBinaryLensing-3.5.0/LICENSE` & `VBBinaryLensing-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `VBBinaryLensing-3.5.0/README.md` & `VBBinaryLensing-3.6.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,65 +1,84 @@
-[![Build Status](https://travis-ci.org/valboz/VBBinaryLensing.svg?branch=master)](https://travis-ci.org/valboz/VBBinaryLensing)
 [![Join the chat at https://gitter.im/VBBinaryLensing/Lobby](https://badges.gitter.im/VBBinaryLensing/Lobby.svg)](https://gitter.im/VBBinaryLensing/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
 
 # VBBinaryLensing
-`VBBinaryLensing` is a tool for forward modelling of gravitational 
-microlensing events using the advanced contour integration method 
-It supports single and binary lenses. 
+`VBBinaryLensing` is a tool for efficient computation in gravitational 
+microlensing events using the advanced contour integration method, supporting single and binary lenses. 
+
+In particular, VBBinaryLensing is designed for the following calculations:
+- **Magnification** by single and binary lenses
+- **Centroid** of the images generated by single and binary lenses
+- **Critical curves and caustics** of binary lenses
+- Complete **light curves** including several higher order effects: limb darkening of the source, binary source, parallax, xallarap, circular and elliptic orbital motion.
+
 The code has been developed by Valerio Bozza, University of Salerno.
 It is written as a C++ library and wrapped as a Python package, the user
 can call the code from either C++ or Python.
 
 The root finding algorithm has been adopted from Jan Skowron & Andy Gould
 (http://www.astrouw.edu.pl/~jskowron/cmplx_roots_sg/)
 and translated to C++ by Tyler M. Heintz and Ava R. Hoag.
 The new Python wrapper has been created by Fran Bartolić in collaboration with Etienne Bachelet and Markus Hundertmark.
 
+VBBinaryLensing is also adopted by several user-friendly modeling platforms for microlensing:
+- [pyLIMA](https://github.com/ebachelet/pyLIMA)
+- [MulensModel](https://github.com/rpoleski/MulensModel)
+- [muLAn](https://github.com/muLAn-project/muLAn)
+
+These platforms offer high-level frameworks for easy modeling of microlensing events. Consider using those codes if you do not want to develop your own modeling or simulation code. On the other hand, if you need direct access to basic functions to include in your own project, this is the right place for you.
+
+A selection of recent reviews about microlensing and its applications can be found [here](/docs/reviews.md).
+
 ## Attribution
 Any use of this code for scientific publications should be acknowledged by citations to the works relevant to your study:
-- [V. Bozza, MNRAS 408 (2010) 2188](https://academic.oup.com/mnras/article/408/4/2188/1420048): general algorithm for binary lensing;
-- [V. Bozza et al., MNRAS 479 (2018) 5157](https://academic.oup.com/mnras/article-abstract/479/4/5157/5050380): BinaryMag2 function, Extended-Source-Point-Lens methods; 
-- [V. Bozza, E. Khalouei and E. Bachelet, arXiv:2011.04780](https://arxiv.org/abs/2011.04780): astrometry, generalized limb darkening, Keplerian orbital motion. 
+- [V. Bozza, MNRAS 408 (2010) 2188](https://ui.adsabs.harvard.edu/abs/2010MNRAS.408.2188B/abstract): general algorithm for binary lensing;
+- [V. Bozza et al., MNRAS 479 (2018) 5157](https://ui.adsabs.harvard.edu/abs/2018MNRAS.479.5157B/abstract): BinaryMag2 function, Extended-Source-Point-Lens methods; 
+- [V. Bozza, E. Khalouei and E. Bachelet, MNRAS 505 (2021) 126](https://ui.adsabs.harvard.edu/abs/2021MNRAS.505..126B/abstract): astrometry, generalized limb darkening, Keplerian orbital motion. 
 
 If specifically relevant to your work, please also cite
 [J. Skowron and A. Gould, arXiv:1203.1034](https://arxiv.org/abs/1203.1034).
  
 
 ## Installation
+
+### Python
+
 The easiest way to install VBBinaryLensing is through `pip`
 ```
 pip install VBBinaryLensing
 ```
 If you want the latest development version from Github, clone this 
 repository and run
 ```
 python setup.py install
 ```
+
+Currently, `VBBinaryLensing` works on Linux, MacOS and python >= 2.7. 
+The python package requires `pybind11` which can be installed with
+```
+pip install pybind11
+```
+The package requires a C++ compiler supporting C++.
+
+### C++
+
 If you just want to use the C++ library, clone this repository, the 
 library files `VBBinaryLensingLibrary.cpp` and
 `VBBinaryLensing.h` are located in in `VBBinaryLensing/lib`. 
 An example usage
 of the C++ code is provided in `examples/cpp_examples` together with
 a sample `Makefile` for compiling the library.
 
 The package also contains the following files:
 - `examples/cpp_examples/instructions.cpp` - Contains working examples and specific instructions for all functions.
 - `VBBinaryLensing/data/ESPL.tbl`  - Pre-calculated table for Extended-source-point-lens
 - `VBBinaryLensing/data/OB151212coords.txt` - Sample file with event coordinates
 - `VBBinaryLensing/data/satellite1.txt` - Sample table for satellite position (Spitzer)
 - `VBBinaryLensing/data/satellite2.txt` - Sample table for satellite position (Kepler)
 
-
-Currently, `VBBinaryLensing` works on Linux, MacOS and python >= 2.7. 
-The python package requires `pybind11` which can be installed with
-```
-pip install pybind11
-```
-The package requires a C++ compiler supporting C++.
-
 ## Example usage
 To check the installation, try:
 ```python
 >>>import VBBinaryLensing
 
 # Initialize the VBBinaryLensing object which contains all functions 
 >>>VBBL = VBBinaryLensing.VBBinaryLensing()
@@ -75,19 +94,17 @@
 >>>print(magnification)
 >>>1.6310924403681109
 ```
 
 Example Jupyter notebooks are included in `examples/python_examples`.
 
 ## Documentation
-We are still working on getting the documentation working online. 
-For now, the vast majority of functions are documented with Python
-docstrings which can be accessed as, for example, `?VBBL.BinaryMag2()` in
-a Jupyter notebook.
+Full [documentation for the use of VBBinaryLensing in C++](/docs/readme.md) is available. This can be a good reference also for Python users. 
 
-## Warning
+Furthermore, the vast majority of functions are documented with Python docstrings which can be accessed as, for example, `?VBBL.BinaryMag2()` in
+a Jupyter notebook.
 
-The python wrapper does not support the user-defined limb-darkening law.
+Note that the python wrapper does not support the user-defined limb-darkening law.
 
 ## License
 VBBinaryLensing is freely available to the community under the 
 GNU Lesser General Public License Version 3 included in this repository.
```

### Comparing `VBBinaryLensing-3.5.0/VBBinaryLensing/data/ESPL.tbl` & `VBBinaryLensing-3.6.0/VBBinaryLensing/data/ESPL.tbl`

 * *Files identical despite different names*

### Comparing `VBBinaryLensing-3.5.0/VBBinaryLensing/data/satellite1.txt` & `VBBinaryLensing-3.6.0/VBBinaryLensing/data/satellite1.txt`

 * *Files identical despite different names*

### Comparing `VBBinaryLensing-3.5.0/VBBinaryLensing/data/satellite2.txt` & `VBBinaryLensing-3.6.0/VBBinaryLensing/data/satellite2.txt`

 * *Files identical despite different names*

### Comparing `VBBinaryLensing-3.5.0/VBBinaryLensing/lib/VBBinaryLensingLibrary.cpp` & `VBBinaryLensing-3.6.0/VBBinaryLensing/lib/VBBinaryLensingLibrary.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// VBBinaryLensing v3.5 (2023)
+// VBBinaryLensing v3.6 (2023)
 //
 // This code has been developed by Valerio Bozza (University of Salerno) and collaborators.
 // Any use of this code for scientific publications should be acknowledged by a citation to:
 // V. Bozza, E. Bachelet, F. Bartolic, T.M. Heintz, A.R. Hoag, M. Hundertmark, MNRAS 479 (2018) 5157
 // If you use astrometry, user-defined limb darkening or Keplerian orbital motion, please cite
 // V. Bozza, E. Khalouei and E. Bachelet (arXiv:2011.04780)
 // The original methods present in v1.0 are described in
@@ -889,27 +889,27 @@
 	rho2 = rho*rho;
 	corrquad *= 6 * (rho2 + 1.e-4*Tol);
 	corrquad2 *= (rho+1.e-3);
 	if (corrquad<Tol && corrquad2<1 && (/*rho2 * s * s<q || */ safedist>4 * rho2)) {
 		Mag = Mag0;
 	}
 	else {
-		Mag = BinaryMagDark(s, q, y1v, y2a, rho, a1, Tol);
+		Mag = BinaryMagDark(s, q, y1v, y2a, rho, Tol);
 	}
 	Mag0 = 0;
 
 	if (y2v < 0) {
 		y_2 = y2v;
 		astrox2 = -astrox2;
 	}
 	return Mag;
 }
 
 
-double VBBinaryLensing::BinaryMagDark(double a, double q, double y1, double y2, double RSv, double a1, double Tolnew) {
+double VBBinaryLensing::BinaryMagDark(double a, double q, double y1, double y2, double RSv, double Tolnew) {
 	static double Mag, Magold, Tolv;
     static double LDastrox1,LDastrox2;
 	static double tc, lc, rc, cb,rb;
 	static int c, flag;
 	static double currerr, maxerr;
 	static annulus *first, *scan, *scan2;
 	static int nannold, totNPS;
@@ -1090,15 +1090,16 @@
 	double Mag,r2,cr2,scr2,a1;
 
 	multidark = true;
 
 	for (int i = 1; i < nfil; i++) {
 		if (a1_list[i] > a1_list[imax]) imax = i;
 	}
-	mag_list[imax] = BinaryMagDark(a, q, y1, y2, RSv, a1_list[imax], Tol);
+	a1 = a1_list[imax];
+	mag_list[imax] = BinaryMagDark(a, q, y1, y2, RSv, Tol);
 
 	for (int i = 0; i < nfil; i++) {
 		if (i != imax) {
 			Mag = 0;
 			a1 = a1_list[i];
 			for (scan = annlist->next; scan; scan = scan->next) {
 				r2 = scan->bin*scan->bin;
@@ -1411,21 +1412,21 @@
 	if (u6*(1+0.003*rho2Tol) > 0.027680640625*rho2Tol*rho2Tol) {
 		Mag = (u2+2)/(u*sqrt(u2+4));
 		if (astrometry) {
 			astrox1 = u * (1 + 1 / (u2 + 2));
 		}
 	}
 	else {
-		Mag = ESPLMagDark(u, rho, a1);
+		Mag = ESPLMagDark(u, rho);
 	}
 	Mag0 = 0;
 	return Mag;
 }
 
-double VBBinaryLensing::ESPLMagDark(double u, double RSv, double a1) {
+double VBBinaryLensing::ESPLMagDark(double u, double RSv) {
 	double Mag = -1.0, Magold = 0., Tolv = Tol;
 	double tc, rb, lc, rc, cb,u2;
 	int c = 0, flag;
 	double currerr, maxerr;
 	annulus *first, *scan, *scan2;
 	int nannold, totNPS = 1;
         double LDastrox1=0.0;
@@ -2877,19 +2878,31 @@
 				if (center->dJ < 0) center->dJ = -center->dJ;
 				if (right->dJ > 0) right->dJ = -right->dJ;
 			}
 		}
 	}
 	if (checkJac != -1) {
 //		printf("\ncheckJac!");
-		_point *scan2;
-		for (scan = Prov->first; scan; scan = scan2) {
-			scan2 = scan->next;
-			Prov->drop(scan);
-			delete scan;
+		if (theta->th < 0) {
+			dJ = 0;
+			for (scan = Prov->first; scan; scan = scan->next) {
+				dJ = dJ+ 1 / fabs(scan->dJ);
+			}
+			if (fabs(dJ.re - 1) < Tol) {
+				checkJac = -1;
+				corrquad = 0;
+			}
+		}
+		if(checkJac!=-1){
+			_point* scan2;
+			for (scan = Prov->first; scan; scan = scan2) {
+				scan2 = scan->next;
+				Prov->drop(scan);
+				delete scan;
+			}
 		}
 	}
 	return Prov;
 }
 
 void VBBinaryLensing::OrderImages(_sols *Sols, _curve *Newpts) {
 	static double A[5][5];
```

### Comparing `VBBinaryLensing-3.5.0/VBBinaryLensing/lib/VBBinaryLensingLibrary.h` & `VBBinaryLensing-3.6.0/VBBinaryLensing/lib/VBBinaryLensingLibrary.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// VBBinaryLensing v3.5 (2023)
+// VBBinaryLensing v3.6 (2023)
 //
 // This code has been developed by Valerio Bozza (University of Salerno) and collaborators.
 // Any use of this code for scientific publications should be acknowledged by a citation to:
 // V. Bozza, E. Bachelet, F. Bartolic, T.M. Heintz, A.R. Hoag, M. Hundertmark, MNRAS 479 (2018) 5157
 // If you use astrometry, user-defined limb darkening or Keplerian orbital motion, please cite
 // V. Bozza, E. Khalouei and E. Bachelet (arXiv:2011.04780)
 // The original methods present in v1.0 are described in
@@ -49,14 +49,15 @@
 namespace VBBinaryLensingLibrary {
 
 	public ref class VBBinaryLensing
 #else
 	class VBBinaryLensing
 #endif
 	{
+	protected:
 		int *ndatasat;
 		double **tsat,***possat;
 		double Mag0, corrquad, corrquad2, safedist;
 		int nim0;
 		double e,phi,phip,phi0,Om,inc,t0,d3,v3,GM,flagits;
 		double Obj[3],rad[3],tang[3],t0old;
 		double Eq2000[3],Quad2000[3],North2000[3];
@@ -98,27 +99,27 @@
 	// Magnification calculation functions.
 
 		double BinaryMag0(double s,double q,double y1,double y2, _sols **Images);
 		double BinaryMag0(double s, double q, double y1, double y2);
 		double BinaryMag(double s,double q,double y1,double y2,double rho,double accuracy, _sols **Images);
 		double BinaryMag(double s,double q ,double y1,double y2,double rho,double accuracy);
 		double BinaryMag2(double s, double q, double y1, double y2, double rho);
-		double BinaryMagDark(double s, double q, double y1, double y2, double rho, double a1,double accuracy);
+		double BinaryMagDark(double s, double q, double y1, double y2, double rho,double accuracy);
 		void BinaryMagMultiDark(double s, double q, double y1, double y2, double rho, double *a1_list, int n_filters, double *mag_list, double accuracy);
 
 	// Limb Darkening control
 		enum LDprofiles { LDlinear, LDquadratic, LDsquareroot, LDlog, LDuser};
 		void SetLDprofile(double(*UserLDprofile)(double), int tablesampling);
 		void SetLDprofile(LDprofiles);
 
 	// ESPL functions
 		void LoadESPLTable(char *tablefilename);
 		double ESPLMag(double u, double rho);
 		double ESPLMag2(double u, double rho);
-		double ESPLMagDark(double u, double rho, double a1);
+		double ESPLMagDark(double u, double rho);
 		double PSPLMag(double u);
 
 
 	// New (v2) light curve functions, operating on arrays
 
 		void PSPLLightCurve(double *parameters, double *t_array, double *mag_array, double *y1_array, double *y2_array, int np);
 		void PSPLLightCurveParallax(double *parameters, double *t_array, double *mag_array, double *y1_array, double *y2_array, int np);
```

### Comparing `VBBinaryLensing-3.5.0/VBBinaryLensing/lib/python_bindings.cpp` & `VBBinaryLensing-3.6.0/VBBinaryLensing/lib/python_bindings.cpp`

 * *Files identical despite different names*

### Comparing `VBBinaryLensing-3.5.0/VBBinaryLensing.egg-info/SOURCES.txt` & `VBBinaryLensing-3.6.0/VBBinaryLensing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `VBBinaryLensing-3.5.0/setup.cfg` & `VBBinaryLensing-3.6.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 author = fran
 author_email = 
 license = BSD 3-Clause
 url = http://astropy.org
 edit_on_github = False
 github_project = astropy/astropy
 install_requires = astropy
-version = 3.5.0
+version = 3.6.0
 minimum_python_version = 3.6
 
 [entry_points]
 astropy-package-template-example = packagename.example_mod:main
 
 [egg_info]
 tag_build =
```

### Comparing `VBBinaryLensing-3.5.0/setup.py` & `VBBinaryLensing-3.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, Extension, find_packages
 from setuptools.command.build_ext import build_ext
 import sys
 import setuptools
 import os
 
-__version__ = '3.5.0'
+__version__ = '3.6.0'
 
 
 class get_pybind_include(object):
     """Helper class to determine the pybind11 include path
 
     The purpose of this class is to postpone importing pybind11
     until it is actually installed, so that the ``get_include()``
```

